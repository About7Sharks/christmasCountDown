<template>
  <div>
    <ul>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
       <li></li>
        <li></li>
         <li></li>
          <li></li>
           <li></li>
            <li></li>
             <li></li>
              <li></li>
    </ul>
  </div>
</template>
<script>
  export default {
    name: 'lights'
  }

</script>
<style scoped>
  ul {
    position: absolute;
    width: 100%;
    margin: 20px 0 0;
    padding: 0;
    border-top: 2px solid #777;
    display: flex;

  }

  ul li {
    list-style: none;
    position: relative;
    top: -20px;
    width: 24px;
    height: 40px;
    border-radius: 50%;
    background: rgba(255, 255, 255, .1);
    margin: 25px;

  }

  ul li::before {
    content: '';
    position: absolute;
    top: -7px;
    left: 7px;
    width: 10px;
    height: 8px;
    background: #444;
  }

  ul li:after {
    content: '';
    position: absolute;
    top: -24px;
    width: 74px;
    height: 26px;
    border-bottom: 2px solid #444;
    border-radius: 50%;
  }

  ul li:last-child:after {
    border-bottom: none;
  }

  ul li:nth-child(3n+1) {
    background: rgb(255, 255, 0, 1);
    animation: animate1 2.5s linear infinite;
  }

  @keyframes animate1 {
    0% {
      background-color: rgb(255, 255, 0, .2);
    }

    50% {
      background-color: rgb(255, 255, 0, 1);
      box-shadow: 0 0 25px rgb(255, 255, 0, 1), 0 0 45px rgb(255, 255, 0, 1)
    }

    100% {
      background-color: rgb(255, 255, 0, .2);
    }
  }

    ul li:nth-child(3n+2) {
      background-color: rgb(255, 0, 255, 1);
    animation: animate2 2.5s linear infinite;
    animation-delay: .9s;
  }

  @keyframes animate2 {
    0% {
      background-color: rgb(255, 0, 255, .2);
    }

    50% {
      background-color: rgb(255, 0, 255, 1);
      box-shadow: 0 0 25px rgb(255, 0, 255, 1), 0 0 45px rgb(255, 0,255 , 1)
    }

    100% {
      background-color: rgb(255, 0, 255, .2);
    }
  }

    ul li:nth-child(3n+3) {
      background-color: rgb(0, 162, 255,1);
    animation: animate3 2.5s linear infinite;
    animation-delay: 1.9s;
  }

  @keyframes animate3 {
    0% {
      background-color: rgb(0, 162, 255,.2);
    }

    50% {
      background-color: rgb(0, 162, 255,1);
      box-shadow: 0 0 25px rgb(0, 162, 255,1), 0 0 45px rgb(0, 162, 255,1)
    }

    100% {
      background-color: rgb(0, 162, 255,.2);
    }
  }
</style>
