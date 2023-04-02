<script lang="ts">
  let counter:number = 12

  const increment = () => {
    counter++
  }

  const incrementTen = () => {
    counter += 10
  }

  const decrement = () => {
    counter--
  } 
  
  const decrementTen = () => {
    counter -=10
  }
</script>

<div class="counter">
  <button on:click={increment} on:dblclick={incrementTen}>+</button>
  <div>{counter}</div>
  <button on:click={decrement} on:dblclick={decrementTen}>-</button>
</div>

<style>
  .counter {
    display: flex;
    justify-content: center;
  }

  .counter > * {
    padding: 10px;
  }
</style>