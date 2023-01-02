
# Utilizando o OpenAI e o Azure Speech Service para criar áudio a partir de dados

### Fluxo 

O fluxo de aplicativo descrito anteriormente tem como intuito automatizar o processo de geração de explicações de versículos bíblicos. Ele faz isso consumindo um JSON com informações sobre os versículos da Bíblia, enviando essas informações para o OpenAI para que ele gere um texto explicativo, e então enviando esse texto para o Azure Speech Service para que ele possa ser convertido em áudio.

O objetivo final é permitir que o aplicativo gere explicações de versículos bíblicos de maneira automatizada, sem a necessidade de intervenção humana. Isso pode ser útil em vários contextos, como em aplicativos de estudo bíblico, podcasts ou programas de rádio cristãos.

1. O aplicativo começa a executar e faz uma solicitação HTTP para obter um JSON de um servidor externo.

2. O servidor envia o JSON de volta para o aplicativo, que então processa as informações contidas no JSON.

3. O aplicativo envia uma solicitação para o OpenAI para gerar um texto com base nas informações contidas no JSON.

4. O OpenAI processa a solicitação e envia o texto gerado de volta para o aplicativo.

5. O aplicativo envia o texto para o Azure Speech Service para que ele possa ser convertido em áudio.

6. O Azure Speech Service processa a solicitação e gera um arquivo de áudio .wav.

7. O aplicativo recebe o arquivo

8. O aplicativo salva o arquivo .wav em seu próprio repositório ou o envia para outro servidor para armazenamento.

9. O aplicativo pode então reproduzir o áudio para o usuário ou exibir o texto gerado pelo OpenAI na interface do usuário.

10. O aplicativo pode continuar a executar esses passos várias vezes, sempre que houver uma nova solicitação de geração de áudio ou texto.



<p align="center">
  <img src="https://user-images.githubusercontent.com/38250160/210195042-c489eba3-60a3-4f8d-b527-2e0598e5451e.png">
</p>
