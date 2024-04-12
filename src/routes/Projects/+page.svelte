<script>
</script>

<h1 class="display grid, justify-items-center"><b>Projects</b></h1>

<div class="grid">

  <div class="card">
    <div class="circle"></div>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed porttitor orci ut sapien rutrum aliquet.</p>
  </div>

  <div class="card">
    <div class="circle"></div>  
    <p>Cras maximus pellentesque nunc sed dictum. Cras accumsan rutrum felis, eu congue velit suscipit sed.</p>
  </div>

  <div class="card">
    <div class="circle"></div>
    <p>Phasellus sit amet mattis nulla, non ornare dui. Aenean consectetur velit vestibulum velit sagittis vehicula.</p>
  </div>
  
</div>


<style>
.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 20px;
}

.card {
  background: #fff;
  padding: 1rem;
  border-radius: 0.5rem;
}

.circle {
 width: 150px; 
  height: 150px;
  border-radius: 50%; 
  background: rgba(0,0,0,0.1);
  margin: 0 auto 20px;
}

p {
	margin-top: 1rem;
}
</style>
