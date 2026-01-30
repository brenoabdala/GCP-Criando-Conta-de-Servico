<h2>GCP - Criando Conta de Serviço </h2>

<p>A <strong>Conta de Serviço</strong> é como um <strong>crachá de acesso</strong> que você emite especificamente para esse funcionário. Esse crachá tem limitações: ele só abre a porta do depósito e nada mais.</p>

<table border="1" width="100%" cellpadding="10" style="border-collapse: collapse; border-color: #e1e4e8;">
  <thead>
    <tr style="background-color: #f6f8fa;">
      <th align="left">Conceito</th>
      <th align="left">Utilidade Real</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Identidade Digital</strong></td>
      <td>É um "e-mail" especial (ex: <code>meu-projeto@id-projeto.iam.gserviceaccount.com</code>) que identifica o seu código perante o Google.</td>
    </tr>
    <tr>
      <td><strong>Segurança</strong></td>
      <td>Se alguém roubar esse "crachá", essa pessoa só terá acesso ao que você permitiu (ex: apenas ler arquivos), e não à sua conta bancária ou outros e-mails.</td>
    </tr>
    <tr>
      <td><strong>Autonomia</strong></td>
      <td>Permite que o seu site ou aplicativo funcione 24h por dia sem que você precise estar logado para autorizar cada ação.</td>
    </tr>
  </tbody>
</table>

<br />

<h3>Funcionamento:</h3>

<p align="center">
  <strong>Seu Código</strong> -> <em>Apresenta o arquivo JSON (Chave)</em> -> <strong>Google Cloud</strong> -> <em>Verifica as permissões do "Crachá"</em> -> <strong>Acesso Liberado ao Bucket</strong>
</p>
<hr />

<h3>Riscos de usar a conta pessoal:</h3>
<ol>
    <li><strong>Risco:</strong> Se você colocar sua senha pessoal no código e alguém ver, sua conta inteira do Google estará em perigo.</li>
    <li><strong>Escalabilidade:</strong> Se você sair da empresa ou mudar de e-mail, o código para de funcionar. A conta de serviço pertence ao projeto, não a você.</li>
</ol>

<p><em>Nota: No Google Cloud, o gerenciamento dessas contas e permissões é feito dentro de uma área chamada <strong>IAM</strong> (Identity and Access Management).</em></p>
