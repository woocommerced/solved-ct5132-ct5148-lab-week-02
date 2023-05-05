Download Link: https://assignmentchef.com/product/solved-ct5132-ct5148-lab-week-02
<br>






<ol>

 <li><strong><sub>Dictionaries</sub></strong>. Use a dict comprehension to invert a dictionary. That is, if in the original dict we have a key-value pair k: v, we should now have v: k.</li>

 <li>Is it possible to have multiple entries in a dict with the same key k? What is the effect of your invert code if there are multiple entries in the original dict with the same <strong><sub>value </sub></strong>v? Think about it, then try it. 3. <strong>Higher-order functions</strong>: we want to create a list containing <em>e<sup>x </sup>∀x ∈ </em>[0<em><sub>.</sub></em>0<em><sub>,</sub></em>0<em><sub>.</sub></em>1<em><sub>,…,</sub></em>1<em><sub>.</sub></em>0]. Use range, lambda, map and of course math.exp to do this.</li>

 <li><strong><sub>Exceptions</sub></strong>. In the following code, check that the user does not request too large a value of <em><sub>n</sub></em>. If they do, raise ValueError with an informative message such as ValueError: Can’t return 7 elements from abcde of length 5. Hint: you could use an f-string to create that string.</li>

</ol>

<strong>def </strong>get_last_n_elements(s, n):

<strong>return </strong>s[-n:]

<ol start="5">

 <li><strong>Itertools</strong>: a <strong>magic square </strong>is an <em>n × n </em>grid containing the numbers 1<em><sub>,</sub></em>2<em><sub>,…n</sub></em><sup>2 </sup>(used exactly once each) such that each row and column sums to the same value. Here is a 3 <em><sub>× </sub></em>3 magic square:</li>

</ol>

(9, 5, 1) (4, 3, 8) (2, 7, 6)

We will generate all magic squares for <em><sub>n </sub></em>= 3. Look up itertools.permutations and use it to generate all permutations of the numbers 1<em><sub>,</sub></em>2<em><sub>,…</sub></em>9. Next, for each permutation p, think of it as a grid, like this:

(p[0], p[1], p[2]) (p[3], p[4], p[5]) (p[6], p[7], p[8])

Check whether the rows and columns sum to the right value, and if so, print it out.

Hint: in Python, you can chain multiple comparisons together, e.g. x == y == z.

1

<ol start="6">

 <li><strong><sub>Generators</sub></strong>: create a generator (a “function” that uses yield) that yields the squares of all the non-negative integers, starting at 0.</li>

 <li>Test it by running for s in sq(): print(s). Of course it creates an infinite loop. To exit the loop, we have to interrupt Python:

  <ul>

   <li>In Spyder, type Ctrl-C in the console</li>

   <li>In Terminal or IPython, type Ctrl-C</li>

   <li>In Jupyter Notebook, go to the Kernel menu and select interrupt.</li>

  </ul></li>

 <li>Without altering your generator, use it to create a for-loop that prints out all the even squares <em><sub>≤ </sub></em> This time, your for-loop could use break to avoid the infinite loop.</li>

</ol>


