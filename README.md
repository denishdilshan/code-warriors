<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!----Navigation Starts-->
    <nav class="navbar navbar-inverse navbar-fixed-top">
        <div class="container">
            <div class="navbar-header">
                <!--Responsive BUtton-->
                <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#navi">
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>

                <h1 style="color: white;margin-top: 10px;" id="myhead">Knowledge Dot</h1>
                </div>
                <div class="collapse navbar-collapse" id="navi">
                    <!--Navigaation menus starts-->
                    <ul class="nav navbar-nav navbar-right">
                        <li><a href="">Home</a></li>
                        <li><a href="">Our Service</a></li>
                        <li><a href="">Works</a></li>
                        <li><a href="">Team</a></li>
                        <li><a href="">About</a></li>
                        <li><a href="">Carrier</a></li>
                        <li><a href=""id="our-location" class="btn-success" data-target="#mymodal" data-toggle="modal">Login/Signup</a></li>

                    </ul>
                    <!---Navigation menus ends-->
                </div>

            </div>
        </div>
    </nav>
    <!----Navigation menus Ends-->

    <!--Slider Section starts-->
    <section class="slider text-center" id="slider">
        <div class="modal-dialog">
            <div class="modal-content">
                <h3 id="login-heading">Login</h3>

                <div class="modal-body">
                    <div class="left-box">
                        <form method="POST" action="validation.php" onsubmit="return validation()">
                        <div class="form-group">
                            <label><i class="fa fa-user fa-2x">
                            </i>Username :</label>
                            <input type="text" autocomplete="off" name="name" class="form-control" id="username" onkeypress="clear()">
                        </i>Password :</label>
                        <input type="password" autocomplete="off" name="password" class="form-control" id="password">

								<span id="perror"><?php 
								if(isset($_SESSION['error']))
								{
									echo "wrong username or password";
								} 
								else{ echo " ";} 
								?>
									

								</span>
								<button id="btn-login" type="submit">Login</button>
								
							</div>
							<div class="register">
								<h2>Don't have an account?&nbsp<span id="create-account"><a href="signup.html">Create</span></a> </h2>
							</div>
							
						</form>
					</div>
					<div class="right-box">
						<span class="signinwith">Sign in With <br> Social Networks</span>

						<button class="social facebook">Log in with Facebook</button>
						<button class="social twitter">Log in with twitter</button>
						<button type="submit" class="social google g-signin2" data-onsuccess="onSignIn()">Log in with gmail</button>
					</div>
						
					</div>
					
						
				</div>
			</div>
			</section>
			

			<!---Slider Section ends------->

			<!---confirm password validation Start------->
                        </div></form>
                    </div>
                </div>
            </div>
        </div>
    </section>
</body>
</html>
