# Dia 31/08/2016 a 05/09/2026
### Projeto: Back in Time
### Plataforma de Tradução: Weblate no Codeberg

Nesta semana de atividades na disciplina, escolhi contribuir para o Back in Time, um utilitário de backup para sistemas baseados em Linux.

Depois de ler sobre a demanda de tradução da aplicação para português, entrei ([github do Back In Time](https://github.com/bit-team/backintime) e li as intruções de contribuição como tradutora. 

Antes de iniciar qualquer alteração, dediquei cerca de uma hora à leitura da documentação do software. O principal mecanismo do projeto consiste em realizar backups eficientes reutilizando arquivos inalterados por meio de hard links. Isso permite economizar espaço em disco entre diferentes versões de cópias de segurança e oferece uma estrutura de recuperação dinâmica e clara para o usuário. O mais interessante é a numeração dessas versões para que se possa fazer a recuperação de arquivos de forma mais dinâmica.

Entre as diretrizes de tradução, estão:
- É proibido o uso de IA para as traduções, visto que ela pode ignorar certos contextos e nuances de um idioma
- Fazer tradução voltada ao público leigo, com o mínimo de jargão tecnológico possível.
- Realizar revisões nas traduções marcadas como "revisão necessária" quando algum tipo de erro de digitação for detectado em sua tradução

Após análise das regras, segui para fazer a conta no [site de tradução](https://codeberg.org) e prossegui à aba de apresentação dos tradutores, onde cada contribuidor colocou seu nome e salvou. A plataforma do Codeberg é bem simples no seu uso geral de observar quais traduções ainda precisam ser feitas, apenas necessitando clicar no ícone de traduzir na seção de "não traduzidos".

Realizei um total semanal de [72 traduções](https://translate.codeberg.org/memory/) (com número que pode aumentar ao longo do avanço dos dias) de textos ao longo dessa semana, precisando parar em muitos momentos devido à necessidade de entender como traduzir certos jargões específicos de ferramentas Linux que nunca utilizei, além de ter que aprender termos que nunca ouvi antes, como os tão mencionados "hard links". As palavras udev (software responsável por gerenciar dispositivos externos, que é um componente do núcleo do Linux), hard link e muitas outras trouxeram desafios que eu, como poliglota entusiasta de idiomas, nunca havia enfrentado. 

Existe sempre o dilema de traduzir para deixar o nome de um componente mais intuitivo e acabar dificultando funcionalidades para quem sempre mexeu nelas sem tradução, claro, mas também existem problemas quando o inglês possui expressões idiomáticas únicas que traduzidas viram jargões técnicos, que provavelmente não seriam bem compreendidos pelo usuário comum. Um desses exemplos emblemáticos da minha jornada de tradução foi a palavra "mount/unmount'. A princípio, observada sem o devido cuidado, vira a palavra "montar", mas como tenho experiência com a língua o suficiente para perceber que a frase em que estava inserida exigia outro significado. Uma pesquisa mais extensa do que as demais me levou a entender que era algo muito específico do fuincionamento dos diretórios Linux. Mount traduzido de forma simples e mais intuitiva, seria "associar um sistema de arquivos a um diretório", unmount seria o efeito oposto, desassociar, tornando o arquivo inacessível. No entanto, as traduções diretas frequentemente eram mais técnicas que isso.

A tradução era algo que eu esperava que fosse simples e rápido, mas a quantidade de traduções e a quantidade de pesquisa envolvida me surpreenderam bastante.

Depois de alguns dias, percebi que seria necessário entrar em contato direto com os desenvolvedores do projeto para tirar minhas dúvidas, porque não sabia que canal usar para entrar em contato, se haviam muitas pessoas ativas na tradução, então enviei essas dúvidas e minha apresentação pessoal pelo e-mail a seguir: 

![e-mail](imagens/{E866E437-FB0E-40BF-A6A4-93D7BD21ADBE}.png)

Esse e-mail foi prontamente respondido no dia seguinte pelo responsável do projeto, Christian Buhtz:

     
          Hello Sara,

          thank you for your message and your efforts to participate.

          I saw your translation activity on translate.codeberg.org. Very well, as
     I can say from my limited perspective as someone who does not not your
     language. ;)

          Am 06.09.2026 04:57 schrieb Sara Leticia Santos Silva:
     > I also wanted to contribute in coding or testing but I have little
     > experience with coding in an existing application.

          Currently testing would be very grade. The second release candidate for
     version 2.0.0 is available.

          https://github.com/bit-team/backintime/releases/tag/v2.0.0-rc2

     > Do your members have a primary way to communicate

          There are not much "members", sadly. If you want to communicate in
     public you could use the mailing list. There are also some folks on the
     Mastodon.

     > and help each other?

          I beg for testers. I modified so many things in 2.0.0 that it need to be
     treated as unstable.

     > I've submitted some but the interface used for these
     > translations are a little confusing and I'm not sure whether there is
     > still
     > translations to do or not.

          Yes the interface (Weblate) is akward somehow. "Portuguese (Brazil)" is
     64% complete. Just press "Translate" and the platform will show strings
     that are untranslated (empty) and already translated strings but marked
     as "Needs editing".
          As I can see from your translation activity, you are the new maintainer
     for "Portuguese (Brazil)". In other words: You are the boss. You an
     decide the details because you are the native speaker.

     > Do you guys intend to offer some kind of translation for the developers
     > that might want to contribute to the GitHub code?

          I don't understand this question. Do you mean translating
     non-user-documentation like README.md and CONTRIBUTING.md?

          Best regards,
          Christian Buhtz
     

Devido à essa resposta, me torneira responsável principal pela tradução da aplicação para português, ganhando funções de 'maintainer' no codeberg, me oferecendo total autoridade para realizar alterações estratégicas de tradução para adaptação do público brasileiro.

Antes de receber a resposta extremamente positiva, já tinha enviado um comentário para tirar dúvidas pela [plataforma](https://translate.codeberg.org/translate/backintime/common/pt_BR/?checksum=5369b3929d2073e0&q=state%3A%3Ctranslated&sort_by=component%2C-priority) sobre alguns padrões de tradução de software que eu achava relevantes pela plataforma do codeberg:
![comentário de tradução com a minha pergunta](imagens/{2527B5FD-57E4-49F1-857C-DE311ABB7166}.png) 

Sobre a qual recebi uma resposta positiva sobre a simplificação da tradução existente anteriormente feita por outro tradutor.

![comentário de resposta de Buhtz](imagens/{47DB92D7-AED8-41B0-A8E8-C11C2B2E3049}.png)

O que me deu confiança de que esta afirmação de que eu seria a principal responsável fosse reiterada.

## Próximos passos

Planejo continuar a tradução da aplicação até que a seção de traduções esteja 100% completa, responder à mensagem do Christian confirmando o interesse em traduzir os arquivos README.md e possivelmente o CONTRIBUTING.md, facilitando a entrada de novos desenvolvedores brasileiros no projeto.

## Considerações

Estou considerando baixar e executar a versão Release Candidate (v2.0.0-rc2) enviada pelo mantenedor para validar as novas traduções em ambiente real e reportar eventuais falhas de interface (layout overflow ou inconsistências), como uma ajuda para quer essa nova versão seja mais estável, mas não sei se compreendo todos os mecanismos de Linux necessários para esse tipo de teste. No entanto, enquanto traduzo, pesquiso e observo a documentação, posso ir estudando sobre o software antes de determinar se consigo efetivamente realizar uma testagem confiável.

Resumo de links:

* [Site de tradução](https://codeberg.org)
* [Github do Back In Time](https://github.com/bit-team/backintime)
* [Comentário específico disponível nessen link com a respota de Buhtz](https://translate.codeberg.org/translate/backintime/common/pt_BR/?checksum=5369b3929d2073e0&q=state%3A%3Ctranslated&sort_by=component%2C-priority)
* [Minhas 72 (ou mais, dependendo de quando o link for aberto) de traduções](https://translate.codeberg.org/memory/)

Todas as imagens de diários estão disponíveis na pasta "imagens". Ao final do semestre, será realizado um README contando sobre o projeto da disciplina de forma mais abrangente.