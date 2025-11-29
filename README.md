<h1>Keylogger Simulado em Python — Projeto Educacional de Cibersegurança</h1>

Este repositório contém um projeto de um Keylogger Simulado desenvolvido em Python como parte do desafio da DIO. 
O objetivo é compreender, de forma segura e controlada, como softwares de captura de teclas funcionam, além de refletir sobre mecanismos de defesa, detecção e prevenção. 
Todo o conteúdo é exclusivamente educacional.

<h3>Funcionalidades implementadas</h3>
<ul>
  <li>Captura de teclas pressionadas pelo usuário</li>
  <li>Registro das teclas em logs/log.txt.</li>
  <li>A cada 60 segundos, os dados coletados são preparados e enviados para o e-mail de destino configurado.</li>
  <li>Após o envio, o registro local é limpo para receber novas entradas.</li>
</ul>
<hr>
<ol>
  <h2><li>Instalando as dependências necessárias</li></h2>
  O projeto utiliza uma biblioteca externa para capturar eventos do teclado.
  <br><br>
  
  ```
  py -m pip install pynput
  ```
  <h2><li>Baixe o repositório:</li></h2>
  Baixe o projeto para sua máquina:
  <br><br>

  ```
  keylogger_email.py
  ```
  <h2><li>Configuração da senha de app na conta Google</li></h2>
  Antes de executar o código, precisamos gerar uma senha do Aplicativo, que é uma senha especial gerada pelo próprio provedor de e-mail para permitir que programas externos — como scripts, softwares ou automações, enviem mensagens sem usar sua senha real da conta.
  No caso do Gmail, você consegue gerar essa senha assim:
  <br><br>
  <ul>
    <li>Ative a Verificação em Duas Etapas</li>
    <li>Vá em Gerenciar sua Conta Google → Segurança.</li>
    <li>Entre em Senhas de app.</li>
    <li>Gere uma nova senha para “Aplicativo Personalizado”.</li>
    <li>O sistema criará uma senha de 16 caracteres.</li>
    <li>É essa senha que você usará no script.</li>
  </ul>
  <br><br>
  Uma forma mais simples é acessar o link abaixo no seu navegador, e gerar a senha.
  <br><br>
  
  ```
  https://myaccount.google.com/apppasswords
  ```

  <h2><li>Ajuste dos dados</li></h2>
  Para utilizar a função de envio automático por e-mail, é necessário configurar os dados de e-mail do arquivo.
  No script, você verá estas variáveis:
  <br><br>
  
  ```
  9. EMAIL_ORIGEM = "seu-email"
  10. EMAIL_DESTINO = "seu-email"
  11. SENHA_EMAIL = "senha-de-app-gerada"
  ```
  O que modificar:<br>
  EMAIL_ORIGEM → O e-mail que será usado para enviar os logs<br>
  EMAIL_DESTINO → O e-mail que irá receber os logs (pode ser o mesmo)<br>
  SENHA_EMAIL → É a senha do aplicativo que foi configurada na etapa anterior

  <h2><li>Execute o Script</li></h2>
  Após instalar as dependências e configurar corretamente o e‑mail e a senha de app, você já pode iniciar o keylogger.
  <br><br>
  No terminal, execute:
  <br><br>

  ```
    py .\keylogger_email.py
  ```

  <h2><li>Reflexão sobre Defesa e Prevenção</li></h2>
    Durante o estudo e implementação deste projeto, foi possível compreender como keyloggers exploram falhas humanas e técnicas para capturar informações sensíveis. 
    <br><br>
    Para prevenir ataques reais, algumas medidas essenciais incluem:
    <br><br>
    <ul>
      <li>Utilizar antivírus </li>
      <li>Monitorar processos desconhecidos em execuçãoMonitorar processos desconhecidos em execução</li>
      <li>Analisar acessos suspeitos a arquivos de sistema</li>
      <li>Manter sistemas atualizados</li>
      <li>Conscientizar usuários sobre engenharia social e phishing</li>
      <li>Usar firewalls e bloqueios de scripts não autorizadosUsar firewalls e bloqueios de scripts não autorizados</li>
      <li>Executar arquivos suspeitos somente em ambientes sandbox</li>
    </ul>
    <br>
    Essas práticas reduzem significativamente o risco de infecções.

  <h2><li>Conclusão</li></h2>
  Este projeto permite entender na prática como funciona a captura de teclas em Python e como esse tipo de técnica pode ser usada tanto de forma legítima quanto maliciosa. <br>
  A implementação reforçou a importância da segurança da informação e de medidas preventivas para proteger sistemas contra ameaças reais.<br>
  O foco principal foi o aprendizado, e todo o desenvolvimento foi feito em ambiente seguro e controlado.


</ol>

