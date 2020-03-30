<template>

  <div class="hello">
    <h1>{{ msg }}</h1>
    
    <h3>Top 6 Algorithms Types</h3>

    <ul class="a">
    <!-- we can use dt instal of li as well. -->

   <li> Recursive Algorithms:</li>
      <dd>Function that repeats itself in order to find the solution
        <pre class="prettyprint">
              Fact(x)
                If x is 0      /*0 is the base value and x is 0 is base case*/
                return 1
                return (x*Fact(x-1))  /* breaks the problem into small problems*/
       </pre>

   </dd>
      <li> Dynamic Programming Algorithms:</li>
          <dd>It remembers the past result and use them to find the new result which means it solves difficult problems by breaking it into subproblems.
            <pre class="prettyprint">
              Fib(n)
                  if n=0
                    return 0
                else
                    prev_Fib=0,curr_Fib=1
                repeat n-1 times  /*if n=0 it will skip*/
                    next_Fib=prev_Fib+curr_Fib   
                    prev_Fib=curr_Fib
                    curr_Fib=new_Fib
                return curr_Fib
                
          </pre>
            </dd>
      <li>Greedy Algorithms:</li>
          <dd>It solves the problem by taking the optimal solution in the local scope and it hopes to find it in the global scope</dd>
      
        <li>Divide and Conquer Algorithm:</li>
            <dd>Divide and conquer consist of two parts first of all it divides the problems into smaller subproblems of the same type and solve them solve them recusively and then combine them to to form the solution of the original problem.</dd>
        <li>Brute Force Algorithm</li>
            <dd>A brute force algorithm simply tries all the possibilities until a satisfactory solution is found.</dd>
        <li>Randomized Algorithm</li>
           <dd>A randomized algorithm uses a random number at least once during the computation to make a decision.</dd>
        <li>Back-tracking Algorithm</li>
            <dd>It divides the problem into 4 main parts. It checks all of the solutions until it finds the desired solution. </dd>
    </ul>
    
    
  
    
  
    <h3>Essential Links</h3>
    

    <footer>
    <ul>
      <dt>Career</dt>
      <dt>About us</dt>
      <dt>Location</dt>
    </ul>
  </footer>
  
  </div>
  
  
</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>



<style scoped>
ul.a{
  list-style-type: circle;
  text-align: left;
}
ul li {
  font-size: 19px;
  color:darkblue
}



</style>
