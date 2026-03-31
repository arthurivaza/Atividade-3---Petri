Agente Escolhido: Agente Reativo com Estado Interno
Para este desafio, optei pela implementação do Agente Reativo com Estado Interno. Diferente de um agente reativo simples, este modelo não decide suas ações baseando-se apenas na percepção imediata, mas também em um histórico de estados passados.

Por que esta escolha?
Conforme o material de aula (página 22), agentes reativos com estado interno são fundamentais quando o ambiente é parcialmente observável ou quando o agente precisa evitar loops infinitos. No contexto do labirinto:

Memória de Visitação: O agente armazena as coordenadas por onde já passou em um conjunto (visitados).

Tomada de Decisão: Ao encontrar um cruzamento, ele prioriza caminhos ainda não explorados.

Backtracking: Se o agente entrar em um beco sem saída, ele utiliza o estado interno para retornar à posição anterior e tentar um novo caminho, garantindo que ele não fique "preso".
