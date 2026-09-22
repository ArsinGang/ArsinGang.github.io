<!DOCTYPE html>
<html lang="fa">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ArsinGang | ورود</title>

<style>
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
}

body{
    min-height:100vh;
    font-family:Tahoma,Arial,sans-serif;
    background:
        radial-gradient(circle at top,#241044 0%,#10051e 45%,#07030d 100%);
    color:white;
    display:flex;
    justify-content:center;
    align-items:center;
}

.container{
    width:100%;
    max-width:430px;
    padding:20px;
}

.logo{
    text-align:center;
    margin-bottom:25px;
}

.logo-box{
    width:75px;
    height:75px;
    margin:auto;
    border-radius:20px;
    display:flex;
    justify-content:center;
    align-items:center;
    background:linear-gradient(135deg,#6d2cff,#20d9ff);
    box-shadow:0 0 30px rgba(102,45,255,.45);
    font-size:27px;
    font-weight:bold;
}

.logo h1{
    margin-top:13px;
    font-size:27px;
}

.logo p{
    margin-top:7px;
    color:#aaa;
    font-size:13px;
}

.card{
    background:rgba(19,8,35,.88);
    border:1px solid rgba(125,65,255,.35);
    border-radius:18px;
    padding:25px;
    box-shadow:0 0 35px rgba(0,0,0,.35);
}

h2{
    text-align:center;
    margin-bottom:20px;
}

.input-group{
    margin-bottom:15px;
}

.input-group label{
    display:block;
    margin-bottom:7px;
    font-size:13px;
    color:#ccc;
}

.input-group input{
    width:100%;
    padding:13px;
    border-radius:10px;
    border:1px solid #3b205d;
    outline:none;
    background:#0d0618;
    color:white;
    font-size:14px;
}

.input-group input:focus{
    border-color:#713cff;
    box-shadow:0 0 10px rgba(113,60,255,.2);
}

.human{
    display:flex;
    align-items:center;
    gap:8px;
    margin:12px 0 18px;
    font-size:13px;
    color:#bbb;
}

.human input{
    width:16px;
    height:16px;
    accent-color:#6d2cff;
}

button{
    width:100%;
    border:none;
    border-radius:10px;
    padding:13px;
    background:linear-gradient(90deg,#6d2cff,#18cfff);
    color:white;
    font-size:15px;
    font-weight:bold;
    cursor:pointer;
    box-shadow:0 0 20px rgba(72,55,255,.2);
}

button:hover{
    opacity:.92;
}

.switch{
    text-align:center;
    margin-top:18px;
    font-size:13px;
    color:#aaa;
}

.switch span{
    color:#55d8ff;
    cursor:pointer;
}

#username,
#humanBox{
    display:none;
}

.message{
    text-align:center;
    margin-top:14px;
    font-size:13px;
    color:#ff7777;
    min-height:18px;
}

.loader{
    position:fixed;
    inset:0;
    background:#08030f;
    display:flex;
    justify-content:center;
    align-items:center;
    z-index:100;
}

.loader div{
    width:40px;
    height:40px;
    border:4px solid #25143b;
    border-top-color:#6d2cff;
    border-radius:50%;
    animation:spin 1s linear infinite;
}

@keyframes spin{
    to{
        transform:rotate(360deg);
    }
}
</style>
</head>

<body>

<div class="loader" id="loader">
    <div></div>
</div>

<div class="container">

    <div class="logo">
        <div class="logo-box">AG</div>
        <h1>ArsinGang</h1>
        <p>به گنگ آرسین خوش اومدی</p>
    </div>

    <div class="card">

        <h2 id="title">ورود به حساب</h2>

        <form id="authForm">

            <div class="input-group" id="usernameBox">
                <label>نام کاربری</label>
                <input
                    type="text"
                    id="username"
                    placeholder="نام کاربری خود را وارد کنید"
                >
            </div>

            <div class="input-group">
                <label>ایمیل</label>
                <input
                    type="email"
                    id="email"
                    placeholder="ایمیل خود را وارد کنید"
                    required
                >
            </div>

            <div class="input-group">
                <label>رمز عبور</label>
                <input
                    type="password"
                    id="password"
                    placeholder="رمز عبور خود را وارد کنید"
                    required
                >
            </div>

            <div class="human" id="humanBox">
                <input type="checkbox" id="human">
                <label for="human">من ربات نیستم</label>
            </div>

            <button type="submit" id="submitBtn">
                ورود
            </button>

        </form>

        <div class="message" id="message"></div>

        <div class="switch">
            <span id="switchText">
                حساب نداری؟ ثبت نام کن
            </span>
        </div>

    </div>
</div>

<script>

const SUPABASE_URL =
"https://lhddjuomukejpvssyhuv.supabase.co";

const SUPABASE_KEY =
"sb_publishable_BL17d9ub-AeaHb8upwVKag_aqjJSQt5";

async function supabaseRequest(path, options = {}){

    const response = await fetch(
        SUPABASE_URL + path,
        {
            ...options,
            headers:{
                "Content-Type":"application/json",
                "apikey":SUPABASE_KEY,
                ...(options.headers || {})
            }
        }
    );

    let data = {};

    try{
        data = await response.json();
    }catch(e){}

    return{
        ok:response.ok,
        status:response.status,
        data:data
    };
}

const form =
document.getElementById("authForm");

const title =
document.getElementById("title");

const usernameBox =
document.getElementById("usernameBox");

const username =
document.getElementById("username");

const humanBox =
document.getElementById("humanBox");

const human =
document.getElementById("human");

const submitBtn =
document.getElementById("submitBtn");

const switchText =
document.getElementById("switchText");

const message =
document.getElementById("message");

let signupMode = false;

function showMessage(text){
    message.textContent = text;
}

function showSignup(){

    signupMode = true;

    title.textContent = "ساخت حساب";

    usernameBox.style.display = "block";
    username.style.display = "block";

    humanBox.style.display = "flex";

    submitBtn.textContent = "ثبت نام";

    switchText.textContent =
        "حساب داری؟ وارد شو";

    username.required = true;
}

function showLogin(){

    signupMode = false;

    title.textContent = "ورود به حساب";

    usernameBox.style.display = "none";
    username.style.display = "none";

    humanBox.style.display = "none";

    submitBtn.textContent = "ورود";

    switchText.textContent =
        "حساب نداری؟ ثبت نام کن";

    username.required = false;
}

switchText.addEventListener(
    "click",
    () => {

        showMessage("");

        if(signupMode){
            showLogin();
        }else{
            showSignup();
        }

    }
);

form.addEventListener(
    "submit",
    async function(e){

        e.preventDefault();

        showMessage("");

        const email =
            document
            .getElementById("email")
            .value
            .trim();

        const password =
            document
            .getElementById("password")
            .value;

        submitBtn.disabled = true;

        if(signupMode){

            if(!human.checked){

                showMessage(
                    "لطفاً تأیید کنید که ربات نیستید."
                );

                submitBtn.disabled = false;

                return;
            }

            const usernameValue =
                document
                .getElementById("username")
                .value
                .trim();

            if(!usernameValue){

                showMessage(
                    "لطفاً نام کاربری را وارد کنید."
                );

                submitBtn.disabled = false;

                return;
            }

            const result =
                await supabaseRequest(
                    "/auth/v1/signup",
                    {
                        method:"POST",

                        body:JSON.stringify({
                            email:email,
                            password:password,

                            data:{
                                username:usernameValue
                            }
                        })
                    }
                );

            if(!result.ok){

                showMessage(
                    result.data?.msg ||
                    result.data?.message ||
                    "ثبت نام انجام نشد."
                );

                submitBtn.disabled = false;

                return;
            }

            showMessage(
                "ثبت نام با موفقیت انجام شد. حالا وارد شوید."
            );

            document.getElementById("email").value =
                email;

            showLogin();

            submitBtn.disabled = false;

            return;
        }

        const result =
            await supabaseRequest(
                "/auth/v1/token?grant_type=password",
                {
                    method:"POST",

                    body:JSON.stringify({
                        email:email,
                        password:password
                    })
                }
            );

        if(!result.ok){

            showMessage(
                result.data?.error_description ||
                result.data?.msg ||
                result.data?.message ||
                "ایمیل یا رمز عبور اشتباه است."
            );

            submitBtn.disabled = false;

            return;
        }

        localStorage.setItem(
            "arsin_user_token",
            result.data.access_token
        );

        if(result.data.refresh_token){

            localStorage.setItem(
                "arsin_user_refresh",
                result.data.refresh_token
            );
        }

        /*
         * اینجا فقط تغییر داده شده:
         * قبلاً:
         * window.location.replace("index.html");
         *
         * الان:
         * صفحه اصلی بدون نمایش index.html
         */
        window.location.replace("./");

    }
);

setTimeout(
    () => {
        document.getElementById("loader").style.display =
            "none";
    },
    500
);

</script>

</body>
</html>
