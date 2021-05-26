# mpd

<hello name="{{ name }}"></hello>
<p>
  Start Play:)
</p>

<html>
<head>
    <!-- load bootstrap css -->
    <link rel="stylesheet" href="http://netdna.bootstrapcdn.com/bootstrap/3.0.3/css/bootstrap.min.css">
    <style>
        body    { padding-top:30px; }
    </style>

    <!-- load angularJS -->
    <script src="http://code.angularjs.org/1.2.6/angular.js"></script>
    <script src="app.js"></script>
</head>

<!-- aplicar app angular e controlador para o nosso body -->
<body ng-app="validationApp" ng-controller="mainController">
    <div class="container">
        <div class="col-sm-8 col-sm-offset-2">

            <!-- PAGE HEADER -->
            <div class="page-header"><h1>AngularJS/Angular Validação de Formulário</h1></div>

            <!-- FORM -->
            <!-- passa a variável se nosso formulário é válida ou inválida -->
            <!-- novalidate isso vai evitar a validação padrão do HTML5, já que vamos fazer isso usando o Angular -->
            <form name="userForm" ng-submit="submitForm(userForm.$valid)" novalidate>

                <!-- NAME -->
                <div class="form-group">
                    <label>Name</label>
                    <input type="text" name="name" class="form-control" ng-model="name" required>
                </div>

                <!-- USERNAME -->
                <div class="form-group">
                    <label>Username</label>
                    <input type="text" name="username" class="form-control" ng-model="user.username" ng-minlength="3" ng-maxlength="8">
                </div>

                <!-- EMAIL -->
                <div class="form-group">
                    <label>Email</label>
                    <input type="email" name="email" class="form-control" ng-model="email">
                </div>
                 <!-- CONFIRMAÇÃO EMAIL -->
                <div class="form-group">
                    <label>Confirmação e_mail</label>
                    <input type="eamil" name=email class="form-control" ng-model="email">
                </div>
                 <!-- SENHA -->
                <div class="form-group">
                    <label>Senha</label>
                    <input type="senha" name=senha class="form-control" ng-model="senha">
                </div>
                 <!-- CONFIRMAÇÃO SENHA -->
                <div class="form-group">
                    <label>Confirmação Senha</label>
                    <input type="eamil senha" name=senha class="form-control" ng-model="email senha">
                </div>
                 <!-- CPF -->
                <div class="form-group">
                    <label>CPF</label>
                    <input type="cpf" name="cpf" class="form-control" ng-model="cpf">
                </div>
                 <!-- EMAIL -->
                <div class="form-group">
                    <label>Cidade</label>
                    <input type="cidade" name=cidade class="form-control" ng-model="cidade">
                </div>
               

                <!-- SUBMIT BUTTON -->
                <button type="submit" class="btn btn-primary">Enviar</button>

            </form>
        </div><!-- col-sm-8 -->
    </div><!-- /container -->
</body>
</html>
<!-- SUBMIT BUTTON -->
                <button type="submit" class="btn btn-primary">Cadastrar</button>
                <div class="container" >
    <a class="links" id="paracadastro"></a>
    <a class="links" id="paralogin"></a>
    
    <div class="content">      
      <!--FORMULÁRIO DE LOGIN-->
      <div id="login">
        <form method="post" action=""> 
          <h1>Login</h1> 
          <p> 
            <label for="email_login">Seu e-mail</label>
            <input id="email_login" name="email_login" required="required" type="text" placeholder="contato@htmlecsspro.com"/>
          </p>
          
          <p> 
            <label for="senha_login">Sua senha</label>
            <input id="senha_login" name="senha_login" required="required" type="password" placeholder="1234" /> 
          </p>
          
          <p> 
            <input type="checkbox" name="manterlogado" id="manterlogado" value="" /> 
            <label for="manterlogado">Manter-me logado</label>
          </p>
          
          <p> 
            <input type="submit" value="Logar" /> 
          </p>
          
          <p class="link">
            Ainda não tem conta?
            <a href="#paracadastro">Cadastre-se no Analista Matheus</a>
          </p>
        </form>
      </div>

      <!--FORMULÁRIO DE CADASTRO PARTICULAR-->
      <div id="cadastro">
        <form method="post" action=""> 
          <h1>Cadastro Particular</h1> 
          
          <p> 
            <label for="nome_cad">Seu nome</label>
            <input id="nome_cad" name="nome_cad" required="required" type="text" placeholder="Luiz Augusto" />
          </p>
          
          <p> 
            <label for="email_cad">Seu e-mail</label>
            <input id="email_cad" name="email_cad" required="required" type="email" placeholder="contato@htmlecsspro.com"/> 
          </p>
          
          <p> 
            <label for="senha_cad">Sua senha</label>
            <input id="senha_cad" name="senha_cad" required="required" type="password" placeholder="1234"/>
          </p>
          
          <p> 
            <input type="submit" value="Cadastrar"/> 
          </p>
          
          <p class="link">  
            Já tem conta?
            <a href="#paralogin"> Ir para Login </a>
          </p>
          
        </form>
      </div>
    </div>
  </div> 
