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

<style>
  @import "../assets/Style/CSS.css";
</style>

<template>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.3.1/dist/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
    <link href='https://fonts.googleapis.com/css?family=Cinzel Decorative' rel='stylesheet'>

    <div class="rightLeft">
        <div class="blocLeft">
            <div class="border">
                <p class="welcome">Welcome !</p>
                <p class="signInUp">Sign up to ARTS</p>
                <p class="happyTo">Happy to meet you !</p>
                <div class="form-group">
                    <label>Email</label> 
                    <input class="form-control" type="email" v-model="email" placeholder="Enter your email" /> 
                </div>
                <div class="form-group">
                    <label>Username</label> 
                    <input class="form-control" v-model="username" placeholder="Enter yout username" />
                </div>
                <div class="form-group">
                    <label>Password</label> 
                    <input class="form-control" type='password' v-model="password" placeholder="Enter your password" />
                </div>
                <div class="form-group">
                    <label>Confirm Password</label> 
                    <input class="form-control" type='password' v-model="repeatPassword" placeholder="Confirm your password" />
                </div>
                <button id="submitButton" type="submit">Sign Up</button>
                <div id="textUnderLoginRegisterButton">
                    <p class="greyText">Already have an account ? <a id="switchRegisterLogin" href="/">Login</a></p>
                </div>
            </div>
        </div>

        <div class="blocRight">
            <p class="arts">ARTS</p>
            <img class="artsLogo" src="../assets/Images/artsLogo.png">
        </div>
    </div>
</template>
