<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<script>
export default {
  data() {
    return {
      email: '',
    }
  }
}
</script>

<template>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.3.1/dist/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
    <link href='https://fonts.googleapis.com/css?family=Cinzel Decorative' rel='stylesheet'>

    <div class="rightLeft">
        <div class="blocLeft">
            <div class="border">
                <p class="welcome">Welcome !</p>
                <p class="signInUp">Sign in to ARTS</p>
                <p class="happyTo">Happy to see you again !</p>
                <div id="googleBtn" class="form-group">
                    <div id="insideGoogleBtn">
                        <img id="googleIcon" src="../assets/Images/googleLogo.png">
                        <span id="buttonText">Continue with Google</span>
                    </div>
                </div>
                <p id="or" class="greyText">or</p>
                <div class="form-group">
                    <label>Email or username</label> 
                    <input class="form-control" v-model="username" placeholder="Enter your email or username" />
                </div>
                <div class="form-group">
                    <label>Password</label> 
                    <input class="form-control" type='password' v-model="password" placeholder="Enter your password" />
                </div>
                <button id="submitButton" type="submit">Login</button>
                <div id="textUnderLoginRegisterButton">
                    <p class="greyText">Don't have an account ? <a id="switchRegisterLogin" href="register">Register</a></p>
                </div>
            </div>
        </div>

        <div class="blocRight">
            <p class="arts">ARTS</p>
            <img class="artsLogo" src="../assets/Images/artsLogo.png">
        </div>
    </div>

    
</template>

<style>
  @import "../assets/Style/CSS.css";

#googleIcon {
    display: inline-block;
    vertical-align: middle;
    width: 42px;
    height: 42px;
}

#buttonText {
    vertical-align: middle;
    padding-left: 5px;
    font-size: 14px;
    font-weight: bold;
    font-family: 'Roboto', sans-serif;
}

#googleBtn {
    background: white;
    color: #333333;
    width: 100%;
    border-radius: 5px;
    border: thin solid #000000;
    box-shadow: 1px 1px 1px grey;
    white-space: nowrap;
}

#googleBtn:hover {
    cursor: pointer;
}

#insideGoogleBtn{
    display: flex;
    align-items: center;
    justify-content: center;
}

#or{
    padding-bottom: 1%;
    padding-top: 1%;
    text-align: center;
    font-size: 18px;
}

</style>