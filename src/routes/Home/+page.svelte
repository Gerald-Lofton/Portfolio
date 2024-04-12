<script>
import Layout from '../+layout.svelte'
</script>
<head>
Home
</head>

<slot name="nav"></slot>


    <h1 class="text-center animate-text" style="text-align: center; text-shadow: 2px 2px #FF0000;">Gerald L.</h1>


<body>
  <p style="text-align: center; text-shadow: 2px 2px red;">Tier 1 Incident Response Analyst</p>  
</body>


<slot name="footer"></slot>

<style>
 body {
    background-color: #2d2d2d;
    color: #fff;
  }
  
  h1 {
    color: #ff7f50;
    text-shadow: 1px 1px #ffd700;
  }
  
  p {
    color: #1e90ff;
  }
</style>
