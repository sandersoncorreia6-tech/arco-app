🏀 ARCO Analytics

ARCO Analytics é uma plataforma de análise estatística e tomada de decisão para o basquete.

O objetivo do projeto é transformar dados brutos de jogos em informações úteis para treinadores, com foco em:

Dado → Contexto → Insight → Decisão

A proposta do ARCO é ir além de um simples aplicativo de estatísticas. O sistema foi pensado para ajudar comissões técnicas a entender melhor jogadores, formações, adversários, tendências e situações de jogo.

---

🎯 Objetivo

Criar uma plataforma semelhante ao conceito de Moneyball aplicado ao basquete, utilizando dados para encontrar padrões e vantagens competitivas que nem sempre são percebidos apenas pela observação tradicional.

O ARCO pretende ajudar treinadores a responder perguntas como:

- Qual quinteto apresenta melhor desempenho?
- Quais jogadores funcionam melhor juntos?
- Qual atleta causa maior impacto quando está em quadra?
- Em quais regiões da quadra a equipe é mais eficiente?
- Onde o adversário apresenta maior vulnerabilidade?
- Quais tendências estão se repetindo nos últimos jogos?
- O que deve ser ajustado para o próximo confronto?

---

👤 Perfil inicial

O projeto possui inicialmente um ambiente preparado para:

Treinador: Adriano Mião
Equipe: Tupã / Monstrinho
Modalidade: Basquete

O sistema está sendo desenvolvido para posteriormente suportar múltiplos treinadores, equipes, categorias e organizações.

---

📊 Principais funcionalidades

Scout de jogo

Registro de eventos durante a partida, incluindo:

- arremessos de 2 pontos;
- arremessos de 3 pontos;
- lances livres;
- assistências;
- rebotes ofensivos;
- rebotes defensivos;
- roubos de bola;
- bloqueios;
- turnovers;
- faltas;
- pontuação adversária.

Cada evento pode ser relacionado aos jogadores presentes em quadra, permitindo análises avançadas de quintetos.

---

📈 Analytics

O ARCO está sendo preparado para trabalhar com métricas como:

- eFG% — Effective Field Goal Percentage;
- TS% — True Shooting Percentage;
- Offensive Rating;
- Defensive Rating;
- Net Rating;
- Turnover Percentage;
- Offensive Rebound Percentage;
- Free Throw Rate;
- Pace;
- Four Factors;
- Clutch Performance;
- On/Off;
- análise de tendências;
- análise por formação.

---

👥 Lineups

O sistema permite evoluir para análises de:

- quintetos;
- trios;
- duplas;
- minutos juntos;
- saldo de pontos;
- eficiência ofensiva;
- eficiência defensiva;
- impacto dos jogadores quando entram ou saem de quadra.

---

🎯 Shot Chart

Visualização dos arremessos realizados durante os jogos para identificar:

- regiões mais eficientes;
- zonas de baixa eficiência;
- preferência ofensiva;
- distribuição de arremessos;
- tendências individuais;
- tendências coletivas.

---

🧠 Insights

O objetivo não é apenas mostrar números.

O ARCO busca transformar números em recomendações práticas para a comissão técnica.

Exemplo:

«"O quinteto A apresenta melhor Net Rating, porém a amostra ainda é pequena."»

«"A equipe apresenta queda de eficiência ofensiva no último período."»

«"O adversário permite maior aproveitamento em determinada região da quadra."»

---

🏆 Competições

O projeto possui estrutura para integração com competições como:

- Federação Paulista de Basketball — FPB;
- Liga de Basketball Centro-Oeste Paulista — LBC.

A proposta é reunir jogos e categorias dentro de um único ambiente.

As integrações com fontes públicas ainda estão em desenvolvimento e podem depender da disponibilidade e estrutura dos sites oficiais.

Para uma futura operação comercial em grande escala, poderá ser necessária uma API oficial ou licenciamento de dados.

---

🎥 Vídeos dos jogos

O ARCO permite associar links de partidas disponíveis no YouTube aos respectivos jogos.

Isso permitirá, futuramente, integrar:

- estatísticas;
- scout;
- vídeo;
- momentos específicos da partida;
- análise técnica;
- análise tática.

---

🤖 Inteligência Artificial

Uma das futuras etapas do ARCO será o desenvolvimento do ARCO Assistant.

O treinador poderá fazer perguntas diretamente aos dados, como:

«"Qual foi nosso melhor quinteto nos últimos cinco jogos?"»

«"Quem teve maior impacto defensivo?"»

«"Onde o adversário mais sofre pontos?"»

«"Qual jogador deveria receber mais minutos?"»

O sistema poderá cruzar estatísticas, contexto, histórico e tamanho da amostra antes de gerar uma recomendação.

---

🧪 Confiança estatística

O ARCO deve evitar conclusões precipitadas.

Uma diferença importante do projeto será considerar:

- tamanho da amostra;
- quantidade de minutos;
- número de posses;
- quantidade de jogos;
- consistência do padrão.

Resultados baseados em poucos minutos ou poucos eventos deverão ser apresentados como tendências, não como certezas.

---

💻 Tecnologia

O projeto utiliza:

- Flutter
- Dart
- Android
- Web
- PWA
- GitHub Actions

A arquitetura foi pensada para permitir que a mesma base de código possa atender:

- Android;
- iPhone/iPad através da versão Web/PWA;
- computadores;
- navegadores modernos.

---

📱 Android

Application ID oficial:

com.arcoanalytics.app

Esse identificador deve permanecer fixo nas próximas versões para manter a continuidade do aplicativo.

---

🔐 Assinatura do aplicativo

As versões oficiais do Android utilizam uma chave de assinatura permanente.

As informações sensíveis não devem ser colocadas neste repositório.

Elas devem permanecer armazenadas nos GitHub Actions Secrets.

Segredos utilizados:

ARCO_KEYSTORE_BASE64
ARCO_KEYSTORE_PASSWORD
ARCO_KEY_ALIAS
ARCO_KEY_PASSWORD

⚠️ Nunca publique:

- arquivo ".jks";
- senhas;
- chave de assinatura;
- arquivo contendo os Secrets.

A perda da chave de assinatura pode impedir atualizações futuras do aplicativo.

---

⚙️ GitHub Actions

O projeto possui automações para gerar as versões oficiais.

Android

Workflow:

ARCO Android Release

Ele pode gerar:

app-release.apk
app-release.aab

APK

Utilizado para instalação direta em dispositivos Android.

AAB

Formato utilizado para futura publicação na Google Play Store.

---

🌐 Web / PWA

O projeto também possui estrutura para compilação Web.

A versão PWA permitirá que o ARCO seja utilizado pelo navegador e instalado como aplicativo em dispositivos compatíveis.

---

📦 Versionamento

O ARCO utiliza versionamento progressivo.

Exemplo:

0.5.0
0.6.0
0.7.0
1.0.0

A versão inicial deste repositório é:

ARCO Analytics v0.5.0

As próximas versões devem manter:

- o mesmo Application ID;
- a mesma chave de assinatura;
- aumento do número da versão.

Assim o Android reconhecerá as versões futuras como atualizações do mesmo aplicativo.

---

🗺️ Roadmap

Entre as próximas etapas planejadas estão:

- banco de dados em nuvem;
- autenticação real de usuários;
- múltiplos treinadores;
- múltiplas equipes;
- sincronização entre dispositivos;
- perfis completos de atletas;
- histórico de temporadas;
- análise avançada de lineups;
- scouting de adversários;
- geração automática de game plans;
- relatórios em PDF;
- dashboards;
- IA para análise estatística;
- integração estatística com vídeos;
- modelos preditivos;
- ARCO Impact Score;
- aplicativo oficial para Android;
- versão Web/PWA;
- futura publicação na Play Store.

---

🏀 Visão do projeto

O ARCO Analytics pretende se tornar um ecossistema completo de inteligência esportiva.

A ideia central é simples:

«Não basta ter os dados. É necessário saber o que eles significam e qual decisão tomar a partir deles.»

ARCO Analytics
Dado. Contexto. Insight. Decisão.
