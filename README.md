<!doctype html>
<html lang="Pt">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/css/bootstrap.min.css" integrity="sha384-B0vP5xmATw1+K9KRQjQERJvTumQW0nPEzvF6L/Z6nronJ3oUOFUFpCjEUQouq2+l" crossorigin="anonymous">
    <style>
        .form-control:invalid{
            border: 1px solid #cc0000; 
        }

    </style>
    <title>FORMULARIO</title>
  </head>
  <body>
      <!-- JUMBOTRON -->
      <!-- ESTE COMPONENTE CRIA UMA ÁREA DE DESTAQUE NA PÁGINA -->
    <div class="jumbotron jumbotron-fluid">
       <div class="container">
                <h1 class="display-4">Ótima escolha</h1>
                <p class="lead">Obrigado por comprar na Fashion Roupas, Preencha o formulario abaixo para concluir sua compra.</p>
       </div>
    </div>
    <div class="container">

        <div class="row">

            <div class="col-md-4">
                <div class="card" style="width: 18rem;">
                    <img src="camisa.jpg" class="card-img-top" alt="camisa">
                    <div class="card-body">
                      <h5 class="card-title">Camisa 1 CR Flamengo</h5>
                      <p class="card-text">Camisa 1 do Flamengo, numero e nome do Bruno Henrique, rei da america</p>
                        <dl>
                            <dt>Produto</dt>
                            <dd>Camiseta</dd>

                            <dt>Cor</dt>
                            <dd>Preta/Vermelha</dd>

                            <dt>Tamanho</dt>
                            <dd>G</dd>
                        </dl>
                    </div>
                </div>
            </div>

            <div class="col-md-8"> 
                <form method="POST" action = "checkout.html">

                    <fieldset>
                        <legend>Dados Pessoais</legend>

                        <div class="form-group">
                            <label for="nome"> Nome Completo </label>
                            <input type="text" name="nome" class="form-control" id="nome" required>
                        </div>

                        <div class="form-group">
                            <label for="email"> E-mail </label>
                            <input type="email" name="email" class="form-control" id="email" placeholder="email@exemplo.com" required> 

                        </div>

                        <div class="form-group">
                            <label for="cpf"> CPF </label>
                            <input type="text" name="cpf" class="form-control" id="cpf" placeholder="000.000.000-00" pattern="\d{3}\.\d{3}\.\d{3}-\d{2}"> 
                        </div>

                        <div class="form-group custom-control custom-checkbox">
                            <input type="checkbox" name="news" id="news" class="custom-control-input"> 
                            <label for="news" class="custom-control-label"> Quero Receber Newsletter </label>
                        </div>


                    </fieldset>

                    <fieldset>
                        <legend>Cartão de Crédito</legend>
                        <div class="form-group">
                            <label for="numero">Numero - CVV</label>
                            <input type="text" name="nrcartao" id="nrcartao" class="form-control">
                        </div>

                        <div class="form-group">
                            <label for="bandeira">Bandeira</label>
                            <select id="bandeira" class="custom-select">
                                <option disabled selected >Selecione uma opção...</option>
                                <option value="master">MasterCard</option>
                                <option value="visa">Visa</option>
                                <option value="express">American Express</option>
                            </select>
                             
                        </div>

                        <div class="form-group">
                            <label for="validade">Validade</label>
                            <input type="month" name="validade" id="validade" class="form-control">
                        </div>

                    </fieldset>

                    <button  type="submit" class="btn btn-primary btn-lg">Confirmar Pedido</button>
                    <br><br><br><br><br><br><br><br>
                    
                </form>
        </div>

    </div>

    <!-- Optional JavaScript; choose one of the two! -->

    <!-- Option 1: jQuery and Bootstrap Bundle (includes Popper) -->
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-Piv4xVNRyMGpqkS2by6br4gNJ7DXjqk09RmUpJ8jgGtD7zP9yug3goQfGII0yAns" crossorigin="anonymous"></script>

    <!-- Option 2: Separate Popper and Bootstrap JS -->
    <!--
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js" integrity="sha384-DfXdz2htPH0lsSSs5nCTpuj/zy4C+OGpamoFVy38MVBnE+IbbVYUew+OrCXaRkfj" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js" integrity="sha384-9/reFTGAW83EW2RDu2S0VKaIzap3H66lZH81PoYlFhbGU+6BZp6G7niu735Sk7lN" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/js/bootstrap.min.js" integrity="sha384-+YQ4JLhjyBLPDQt//I+STsc9iw4uQqACwlvpslubQzn4u2UU2UFM80nGisd026JF" crossorigin="anonymous"></script>
    -->
  </body>
</html>
