<template>
  <div class="home">
    <div class="container">
      <h1 class="title">HobbyMate</h1>
      <button class="chat-btn">Chat In Your Browser</button>
      <img src="../assets/Saly-1.svg">
    </div>


    <div class="panel">
      <h1>Talk like never before</h1>
      <p>HobbyMate is free and crossplatform
        system working with browser technology 
        so that it can work on most devices that support 
        browser
      </p>
      <img src="../assets/Saly-43.svg">
      <div class="circle"></div>
    </div>

    <div class="container2">
      <h1 class="sub-title">Why HobbyMate?</h1>
      <div class="innerCont">
        <div class="msg-bubble"><p class="why-text">HobbyMate will always be free to use</p></div>
        <div class="msg-mid-bubble"><p class="why-text">No need to register if you need to chat</p></div>
        <div class="msg-bubble"><p class="why-text">Fast and easy modern interface</p></div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home'
}
</script>


<style lang="scss">

.container{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 700px;
  background: #F5D0B8;


  .title{
    font-size: 2rem;
    margin-top: 130px;
  }

  .chat-btn{
    background: #E65C34;
    color: #fff;
    border: 0;  
    border-radius: 8px;
    padding: 17px;
    margin: 0 auto;
    cursor: pointer;
  }

  img{
    width: 500px;
    height: 500px;
    margin: 0 auto;
    z-index: 1;
  }
}

.panel{
  display: flex;
  flex-direction: column;
  justify-content: center;
  background: #fff;
  border-radius: 30px;
  width: 550px;
  height: 600px;
  margin: auto;
  position: relative;
  left: 0;
  right: 0;
  top: -50px;

  p{
    width: 80%;
    margin: 0 auto;
  }

  img{
    width: 300px;
    margin: 0 auto;
  }

  .circle{
    background: #F5D0B8;
    border-radius: 100%;
    height: 350px;
    width: 350px;
    position: absolute;
    z-index: -1;
    left: -200px;
    top: 350px;
  }
}

.container2{
  width: 550px;
  margin: auto;

  .sub-title{
    font-size: 1.8rem;
    margin: 100px 0 50px 0;
  }

  .innerCont{
    display: flex;
    flex-direction: column;
    gap: 20px;

    .msg-bubble, .msg-mid-bubble{
      width: 80%;
      height: 90px;
      background: #fff;
      border-radius: 30px;
    }

    .msg-mid-bubble{
      align-self: flex-end;
    }

    .why-text{
      display: flex;
      justify-content: center;
      margin: 0;
      align-items: center;
      height: 100%;
    }
  }

}


@media only screen and (max-width: 600px) {
.container{

  img{
    width: 300px;
    height: auto;
    margin: 0;
  }
}

.panel{
  width: 85%;

  img{
    width: 55%;
  }
}

.innerCont{
  width: 85%;
  margin: auto;
}

}

</style>