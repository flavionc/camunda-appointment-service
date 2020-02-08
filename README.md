# Relatório do uso do Camunda para criação de um Sistema de Agendamento de serviços para o Governo do Estado do Ceará.

Foi desenvolvido uma modelagem genérica, utilizando o Camunda Modeler, para simular o processo de agendamento dos serviços de consulta médica, consulta odontológica e renovação de CNH.

A aplicação do usuário foi criada usando o próprio Camunda Tasklist que se conecta com o servidor do Camunda e sincroniza com o processo. Com isso o gestor do processo é capaz de acompanhar o estado em que se encontra o fluxo, identificar de forma mais simples e visual a presença de gargalos, além de conseguir também prever sub ou sobre utilização de recursos.

Foi ativado o recurso do Heatmap (disponível na versão Enterprise), permitindo acompanhar as zonas do processo que mais são percorridas.


## Integrantes:
- Flávio Carneiro
- Lucas Peres
- Saulo Maia
- Victor Lage


## Versões utilizadas:
Camunda Modeler 3.6.0
Camunda Enterprise Platform 7.13.0-alpha1-ee - 30-days Trial

## Pontos positivos

- Fornece uma visão clara do processo modelado, uma vez que a interface do próprio Camunda possui uma funcionalidade de “cockpit” que permite o administrador, através de uma auxílio visual do modelo BPMN ser capaz de identificar desde o estado atual de uma instância de usuário no sistema até uma visão ampla com de gráficos de calor que possibilitam mostrar gargalos no fluxo do sistema.

- Permite, através de sua interface de tasklist, gerar um simples protótipo para experimentar e validar o fluxo do(s) processo(s) desenvolvido(s), testando as permissões e atribuições das atividades entre diversos grupos de usuários

## Pontos negativos

- Erros do Camunda Modeler não são claros e explicativos;

- A documentação do API REST de Camunda poderia fornecer um resumo breve sobre do que se trata cada endpoint. A forma atual da  documentação mostra do que se trata o endpoint apenas ao clicá-lo. 

## Lições aprendidas

- Necessidade de conhecer mais a fundo o Camunda;

- A modelagem de processo deve acompanhar a aplicação;
