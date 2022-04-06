<template>
  <div id="login-div">
        <div  class="login">
                <div class="heading-content">
                    BKExam
                </div>
                <form  id="loginForm">
                    <div class="form-floating mb-3">
                        <input type="email" class="form-control input-content" id="floatingInput" placeholder="User or email">
                        <label for="floatingInput" class="content-inpt">Tài khoản hoặc email</label>
                    </div>
                    <div class="form-floating">
                        <input type="password" class="form-control input-content" id="floatingPassword" placeholder="Password">
                        <label for="floatingPassword" class="content-inpt">Mật khẩu</label>
                    </div>
                    <div class="button-login">
                        <button type="submit"  class="js-login">Đăng nhập</button>
                    </div>
                </form>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>

#login-div{
    background-image: url("@/assets/img-back.jpg");
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-content: center;
}
.login{
    background-color: var(--clrofbackground);
    width: 400px;
    height: 350px;
    margin-top: 180px ;
    opacity: 0.9;
}
.heading-content{
    color: #fff;
    font-size: xx-large;
    text-align: center;
    margin: 24px 0;
}
.users{

}
.form-floating{
    margin: 12px 24px;
}
.button-login{
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    margin-top: 88px;  
}
.button-login button{
    padding: 12px 28px;
}  
.button-login button:hover{
    opacity: 0.6;
}
</style>