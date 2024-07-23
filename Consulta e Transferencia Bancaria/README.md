# Desafio
Criar api de Consulta e transferencia bancaria

## Requisitos de negocio
1. Buscar nomde de cliente em api de cadastro (Mock)
2. Validar se a conta corrente esta ativa
3. Validar se o cliente possui limite disponivel na conta corrente
4. Validar se excedeu limite diario de 1k
5. Apos transferencia, eh necessario notificar o BACEN (Mock)  de forma sincrona que a transacao foi executada com sucesso

## Arquitetura
1. Proposta de escalonamento em caso de oscilacao de carga
2. Proposta de observability
3. Justificar escolha de banco de dados
4. Justificar estrategia para casos de falha

## Desenvolvimento
1. Suportar TPS de 6k com latencia <100ms
2. A API do BACEN pode responder 429 pois possui rate limit.
3. Impedir que falhas momentaneas impactem a experiencia do cliente
4. Ser desenvolvida em JAVA/Springboot
5. Testes unitarios e automatizados
6. Explorar desing patterns
7. Implementar padroes de resiliencia