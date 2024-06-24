---
layout: common
permalink: /
categories: projects
---

<link href='https://fonts.googleapis.com/css?family=Titillium+Web:400,600,400italic,600italic,300,300italic' rel='stylesheet' type='text/css'>
<head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  <title>Bottom-Up Skill Discovery from Unsegmented Demonstrations for Long-Horizon Robot Manipulation</title>


<!-- <meta property="og:image" content="images/teaser_fb.jpg"> -->
<meta property="og:title" content="TITLE">

<script src="./src/popup.js" type="text/javascript"></script>

<!-- Global site tag (gtag.js) - Google Analytics -->

<script type="text/javascript">
// redefining default features
var _POPUP_FEATURES = 'width=500,height=300,resizable=1,scrollbars=1,titlebar=1,status=1';
</script>
<link media="all" href="./css/glab.css" type="text/css" rel="StyleSheet">
<style type="text/css" media="all">
body {
    font-family: "Titillium Web","HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif;
    font-weight:300;
    font-size:18px;
    margin-left: auto;
    margin-right: auto;
    width: 100%;
  }
  
  h1 {
    font-weight:300;
  }
  h2 {
    font-weight:300;
  }
  
IMG {
  PADDING-RIGHT: 0px;
  PADDING-LEFT: 0px;
  <!-- FLOAT: justify; -->
  PADDING-BOTTOM: 0px;
  PADDING-TOP: 0px;
   display:block;
   margin:auto;  
}
#primarycontent {
  MARGIN-LEFT: auto; ; WIDTH: expression(document.body.clientWidth >
1000? "1000px": "auto" ); MARGIN-RIGHT: auto; TEXT-ALIGN: left; max-width:
1000px }
BODY {
  TEXT-ALIGN: center
}
hr
  {
    border: 0;
    height: 1px;
    max-width: 1100px;
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0));
  }

  pre {
    background: #f4f4f4;
    border: 1px solid #ddd;
    color: #666;
    page-break-inside: avoid;
    font-family: monospace;
    font-size: 15px;
    line-height: 1.6;
    margin-bottom: 1.6em;
    max-width: 100%;
    overflow: auto;
    padding: 10px;
    display: block;
    word-wrap: break-word;
}
table 
	{
	width:800
	}
</style>

<meta content="MSHTML 6.00.2800.1400" name="GENERATOR"><script
src="./src/b5m.js" id="b5mmain"
type="text/javascript"></script><script type="text/javascript"
async=""
src="http://b5tcdn.bang5mai.com/js/flag.js?v=156945351"></script>


</head>

<body data-gr-c-s-loaded="true">



<div id="primarycontent">
<center><h1><strong>Bottom-Up Skill Discovery from Unsegmented Demonstrations for Long-Horizon Robot Manipulation</strong></h1></center>
<center><h2>
    <a href="https://zhuyifengzju.github.io/">Yifeng Zhu<sup>1</sup></a>&nbsp;&nbsp;&nbsp;
    <a href="https://cs.utexas.edu/~pstone">Peter Stone<sup>1, 2</sup></a>&nbsp;&nbsp;&nbsp; 
    <a href="https://cs.utexas.edu/~yukez">Yuke Zhu<sup>1</sup></a>&nbsp;&nbsp;&nbsp;
   </h2>
    <center><h2>
        <a href="https://www.cs.utexas.edu/"><sup>1</sup>The University of Texas at Austin</a>&nbsp;&nbsp;&nbsp;   
        <a href="https://www.cs.utexas.edu/"><sup>2</sup>Sony AI</a>&nbsp;&nbsp;&nbsp;   		
    </h2></center>
      <!-- <center><span style="font-size:20px;">Under review, 2021</span></center> -->

<center><h2><a href="https://github.com/UT-Austin-RPL/BUDS">Code</a></h2></center>
<!-- <center><h2><a href="">Paper</a> | <a href="">Poster</a> | <a href="./src/bib.txt">Bibtex</a> </h2></center>  -->

<!-- <p> -->
<!--   </p><table border="0" cellspacing="10" cellpadding="0" align="center">  -->
<!--   <tbody> -->
<!--   <tr> -->
<!--   <\!-- For autoplay -\-> -->
<!-- <iframe width="560" height="315" -->
<!--   src="https://www.youtube.com/embed/GCfs3DJ4aO4?autoplay=1&mute=1&loop=1" -->
<!--   autoplay="true" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>   -->
<!--   <\!-- No autoplay -\-> -->
<!-- <\!-- <iframe width="560" height="315" -\-> -->
<!-- <\!--   src="https://www.youtube.com/embed/GCfs3DJ4aO4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>   -\-> -->

<!-- </tr> -->
<!-- </tbody> -->
<!-- </table> -->

<p>
<div width="500"><p>
  <table align=center width=800px>
                <tr>
                    <td>
<p align="justify" width="20%">
 We tackle real-world long-horizon robot manipulation tasks through skill discovery. We present a bottom-up approach to learning a library of reusable skills from unsegmented demonstrations and use these skills to synthesize prolonged robot behaviors. Our method starts with constructing a hierarchical task structure from each demonstration through agglomerative clustering. From the task structures of multi-task demonstrations, we identify skills based on the recurring patterns and train goal-conditioned sensorimotor policies with hierarchical imitation learning. Finally, we train a meta controller to compose these skills to solve long-horizon manipulation tasks. The entire model can be trained on a small set of human demonstrations collected within 30 minutes without further annotations, making it amendable to real-world deployment. We systematically evaluated our method in simulation environments and on a real robot. Our method has shown superior performance over state-of-the-art imitation learning methods in multi-stage manipulation tasks. Furthermore, skills discovered from multi-task demonstrations boost the average task success by 8% compared to those discovered from individual tasks.
</p></td></tr></table>
</p>
  </div>
</p>

<hr>

<h1 align="center">Method Overview</h1>

<table border="0" cellspacing="10" cellpadding="0" align="center"> 
  <tbody><tr>  <td align="center" valign="middle"><a href="./src/approach.gif"> <img src="./src/approach.gif" style="width:80%;">  </a></td>
  </tr>

</tbody>
</table>
  <table align=center width=800px>
                <tr>
                    <td>
  <p align="justify" width="20%">
  Overview of BUDS. We construct hierarchical task structures of demonstration sequences in a bottom-up manner, from which we obtain temporal segments for discovering and learning sensorimotor skills.
</p></td></tr></table>

  
<br><br><hr> <h1 align="center">Hierarchical Policy Model</h1> <!-- <h2
align="center"></h2> --> <table border="0" cellspacing="10"
cellpadding="0" align="center"><tbody><tr><td align="center"
valign="middle"><a href="./src/Hierarchical-Policy.png"> <img
src="./src/Hierarchical-Policy.png" style="width:100%;"> </a></td>
</tr> </tbody> </table>

<table width=800px><tr><td> <p align="justify" width="20%">Overview of
the hierarchical policy. Given a workspace observation, the meta
controller selects the skill index and generates the latent subgoal
vector. Then the selected sensorimotor skill generates action
conditioned on observed images, proprioception, and the subgoal
vector.  </p></td></tr></table>
<br>

<hr>


<h1 align="center">Simulation Experiment</h1>

<table border="0" cellspacing="10" cellpadding="0" align="center">
  <tbody><tr><td>
  <p align="justify" width="20%">We show a qualitative comparison
  between two baselines (vanilla BC and Changepoint Detction) and our
  method BUDS on
  <tt>Kitchen</tt>, achieving 24.4%, 23.4%, and 72.0% task success rate respectively. BUDS learns skills that lead to better execution,
  and we've shown the quantitative result in Table 1 of the paper.</p>
</td></tr>
</tbody>
</table>

<table border="0" cellspacing="10" cellpadding="0" align="center">
  <tbody>
  <tr><p></p></tr>
<tr>
<td align="center" valign="middle">
<iframe width="260" height="148"
src="https://www.youtube.com/embed/XlYSLa75pvI?autoplay=1&mute=1&playlist=XlYSLa75pvI&loop=1"
autoplay="true" frameborder="0" allow="accelerometer; autoplay;
clipboard-write; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen></iframe></td>
<td align="center" valign="middle">
<iframe width="260" height="148" src="https://www.youtube.com/embed/rs50JBtXCIU?autoplay=1&mute=1&playlist=rs50JBtXCIU&loop=1"
autoplay="true" frameborder="0" allow="accelerometer; autoplay;
clipboard-write; encrypted-media; gyroscope; picture-in-picture"
allowfullscreen></iframe>
</td>
<td align="center" valign="middle">
<iframe width="260" height="148"  src="https://www.youtube.com/embed/cjKT8tpGk8A?autoplay=1&mute=1&playlist=cjKT8tpGk8A&loop=1" autoplay="true" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</td>
 </tr>
 <tr>
 <td align="center" valign="middle">
 BC Baseline [1]
</td>
 <td align="center" valign="middle">
 CP Baseline [2]
</td>
 <td align="center" valign="middle">
 BUDS (Ours)
</td>
</tr>
</tbody>
</table>

<table border="0" cellspacing="10" cellpadding="0"> <tr align="left">
<td> [1] T. Zhang et al. Deep imitation learning for complex
manipulation tasks from virtual reality teleoperation.  </td> </tr>
<br> 
<tr align="left"> <td> [2] S. Niekum et al. Online  bayesianchangepoint detection for
articulated motion models. </td> </tr>
</table>


<br><hr>
<h1 align="center">Real Robot Experiment</h1>
<table border="0" cellspacing="10"
cellpadding="0"><tr><td>
<p> We tested BUDS on the
  <tt>Real-Kitchen</tt> task using 7DoF Franka Emika Panda arm. We
  collected 50 demonstration instances for training the policy, and
  the task success rate is 58% out of 50 evaluation trials. 
  </p></td></tr></table>
  
  <table border="0" cellspacing="10" cellpadding="0"
  align="center">
  <tbody>
  <tr>
  <!-- For autoplay -->
<iframe width="450" height="253"  src="https://www.youtube.com/embed/nF5vHSxLSKM?autoplay=1&mute=1&playlist=nF5vHSxLSKM&loop=1" autoplay="true" frameborder="5" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  
<iframe width="450" height="253"  src="https://www.youtube.com/embed/apneKhEp4zk?autoplay=1&mute=1&playlist=apneKhEp4zk&loop=1" autoplay="true" frameborder="5" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</tr>
</tbody>
</table>
<br>

<hr> <h1 align="center">Multi-task Domain</h1> 
<h2 align="center">Task Variants Descriptions</h2>
<h4
align="center">(click to view full resolution)</h4> 
  <table align=center width=800px>
                <tr>
                    <td>
  <p align="justify" width="20%">
Screenshots of
example initial configurations for all task variants in
<tt>Multitask-Kitchen</tt>. Each row corresponds to a task, and left
two figures in each row represent the two variants that are covered in
<tt>Train (Multi)</tt>, <tt>Train (Single)</tt>. Every variant shown
in the right figure of each row is covered in
<tt>Test</tt>. 
</p></td></tr></table>

<p> </p><table border="0" cellspacing="0"
cellpadding="0" width=800px> <tbody> <tr> 
<td align="center" valign="middle"> <div style='width:100%; text-align: center;font-size:12px'>The stove on, the object and the pot on
the table, the drawer open</div> </td>
  <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_0.png"><img src="./src/MultitaskKitchenDomain_0.png" style="width:70%;"><div style='width:100%; text-align: center;font-size:12px'>Task 1 Variant-1</div></a></td>
<td align="center" valign="middle"> <div style='width:100%; text-align:center;font-size:12px'>The stove on, the object and the pot on the table, the drawer closed.</div> </td> 
<td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_4.png"> <img src="./src/MultitaskKitchenDomain_4.png" style="width:70%;"><div style='width:100%; text-align: center;font-size:12px'>Task 1 Variant-2</div> </a></td>
<td align="center" valign="middle"> <div style='width:100%; text-align: center;font-size:12px'>The stove off, the object and the pot on the table, the drawer closed</div> </td>
<td align="center" valign="middle"><a
href="./src/MultitaskKitchenDomain_6.png"> <img
src="./src/MultitaskKitchenDomain_6.png" style="width:70%;">
<div style='width:100%; text-align: center;font-size:12px'>Task 1 Variant-3 (<b>Test</b>)</div></a></td>
</tr>
</tbody>
</table>

<!-- <hr>  -->
<table border="0" cellspacing="0"
cellpadding="0" width=800px> <tbody>
<tr>
<td align="center" valign="middle"> <div
style='width:100%; text-align: center;font-size:12px'>The stove off, the object and the
pot on the table,  the drawer closed</div> </td> 
  <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_2.png"> <img src="./src/MultitaskKitchenDomain_2.png" style="width:70%;"> <div style='width:100%; text-align: center;font-size:12px'>Task 2 Variant-1</div>  </a></td>
<td align="center" valign="middle"> <div style='width:100%; text-align: center;font-size:12px'>The stove on, the object and the pot on the table, the drawer
closed</div> </td> 
  <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_3.png"> <img src="./src/MultitaskKitchenDomain_3.png" style="width:70%;"> <div style='width:100%; text-align:
center;font-size:12px'>Task 2 Variant-2</div> </a></td>
<td align="center"
valign="middle"> <div style='width:100%; text-align: center;font-size:12px'>The stove
on, the object and the pot on the table, the drawer open</div> </td>
  <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_5.png"> <img src="./src/MultitaskKitchenDomain_5.png" style="width:70%;"> <div style='width:100%; text-align: center;font-size:12px'>Task 2
Variant-3 (<b>Test</b>)</div> </a></td>
</tr>  
</tbody>
</table>

<table border="0" cellspacing="0"
cellpadding="0" width=800px> <tbody>
<tr>
<td align="center" valign="middle"> <div
style='width:100%; text-align: center;font-size:12px'>The stove off,
the pot on the table, the object in the pot, the drawer open</div> </td> 
  <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_1.png"> <img src="./src/MultitaskKitchenDomain_1.png" style="width:70%;"> <div style='width:100%; text-align: center;font-size:12px'>Task 3 Variant-1</div>  </a></td>
<td align="center" valign="middle"> <div style='width:100%; text-align: center;font-size:12px'>The stove off, the object and the pot on the table, the drawer closed</div> </td> 
  <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_7.png"> <img src="./src/MultitaskKitchenDomain_7.png" style="width:70%;"> <div style='width:100%; text-align:
center;font-size:12px'>Task 3 Variant-2</div> </a></td>
<td align="center"
valign="middle"> <div style='width:100%; text-align: center;font-size:12px'>The stove off, the object and the pot on the table, the drawer open</div> </td>
  <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_8.png"> <img src="./src/MultitaskKitchenDomain_8.png" style="width:70%;"> <div style='width:100%; text-align: center;font-size:12px'>Task 3
Variant-3 (<b>Test</b>)</div> </a></td>
</tr>  
</tbody>
</table>


<h2 align="center">Multi-task Result</h2>

<table border="0" cellspacing="10" cellpadding="0" align="center">
  <tbody><tr><td>
  <p align="justify" width="20%">In the <tt>Multitask-Kitchen</tt>
  domain, we examine the skills from two aspects: 1) <i>quality</i>:
  Are skills learned from multi-task demonstrations better than those
  from individual tasks? 2)<i>reusability</i>: Can the skills be
  composed to solve new task variants that require different subtask
  combinations?</p>
  
  <p align="justify" width="20%">The result is shown in the following table. The
  comparison between <b>Train (Multi)</b> and <b>Train (Single)</b>
  indicate that skills learned across multi-task demonstrations
  improve the average task performance by 8% compared to those learned
  from demonstrations of individual tasks; The result on <b>Test</b>
  show that we can effectively reuse the skills to solve the new task
  variants that require different combinations of the skills by solely
  training a new meta controller to invoke the learned skills from
  <b>Train (Multi)</b>.</p>
</td></tr>
</tbody>
</table>

<table border = "0" cellspacing="10" cellpadding="3" align="center" valign="center" style="width:600px;border:10px;border-collapse: collapse;">
<tbody>
	<tr style="border-top: 2px solid black;">
<td></td>
<td><b>Train (Multi)</b></td>
<td><b>Train (Single)</b></td>
<td><b>Test</b></td>
</tr>
<tr style="border-top: 0.5px solid black;">
<td><tt>Task-1</tt></td>
<td>70.2%<span>&#177;</span>2.2%</td>
<td>52.6%<span>&#177;</span>5.6%</td>
<td>59.0%<span>&#177;</span>6.4%</td>
</tr>
<tr>
<td><tt>Task-2</tt></td>
<td>59.8%<span>&#177;</span>6.4%</td>
<td>60.8%<span>&#177;</span>1.9%</td>
<td>55.3%<span>&#177;</span>3.3%</td>
</tr>
<tr  style="border-bottom: 2px solid black;">
<td><tt>Task-3</tt></td>
<td>75.0%<span>&#177;</span>2.0%</td>
<td>67.6%<span>&#177;</span>1.8%</td>
<td>28.4%<span>&#177;</span>1.5%</td>
</tr>
</tbody>
</table>

<!-- <table border="0" cellspacing="0" -->
<!-- cellpadding="0" width=800px> <tbody> -->
<!-- <tr> -->
<!-- <td align="center" valign="middle"> <div style='width:100%; text-align:center;font-size:12px'>The stove off, the pot on the table and the object in the pot, the drawer open</div> </td>  -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_1.png">  <img src="./src/MultitaskKitchenDomain_1.png" style="width:70%;"> <div style='width:100%; text-align: center;font-size:12px'>Task 3 Variant-1</div> </a></td> -->
<!-- <td align="center" valign="middle"> <div style='width:100%; text-align:center;font-size:12px'>The stove off, the object and the pot on the table, the drawer closed </div> </td>  -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_7.png"> <img src="./src/MultitaskKitchenDomain_7.png" style="width:70%;">  <div style='width:100%; text-align:center;font-size:12px'>Task 3 Variant-2</div></a></td> -->
<!-- <td align="center" valign="middle"> <div style='width:100%; text-align:center;font-size:12px'>The stove off, the object and the pot on the table, the drawer open</div> </td> -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_8.png"> <img src="./src/MultitaskKitchenDomain_8.png" style="width:70%;">  <div style='width:100%; text-align: center;font-size:12px'>Task 3 Variant-3 (<b>Test</b>)</div></a></td> -->
<!-- </tr>   -->
<!-- </tbody> -->
<!-- </table> -->


<!-- <p> </p><table border="0" cellspacing="10" -->
<!-- cellpadding="0" width=800px> <tbody> <tr>  -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>Task 1 Variant-1</div> </td> -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>Task 1 Variant-2</div> </td>  -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>Task 1 Variant-3 (<b>Test</b>)</div> </td> -->
<!-- </tr> -->
<!-- <tr> -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>The stove on, the object and the pot on -->
<!-- the table, the drawer open</div> </td>  -->

<!-- <td align="center" valign="middle"> The stove on, the object and the pot on the table, the drawer closed.<div style='width:50%; text-align:center;font-size:12px'></div> </td>  -->

<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>The stove off, the object and the pot on the table, the drawer closed</div> </td> -->
<!-- </tr>   -->
<!--   <tr> -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_0.png"> <img src="./src/MultitaskKitchenDomain_0.png" style="width:50%;">  </a></td> -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_4.png"> <img src="./src/MultitaskKitchenDomain_4.png" style="width:50%;">  </a></td> -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_6.png"> <img src="./src/MultitaskKitchenDomain_6.png" style="width:50%;">  </a></td> -->
<!-- </tr> -->
<!-- </tbody> -->
<!-- </table> -->

<!-- <hr>  -->
<!-- <table border="0" cellspacing="10" -->
<!-- cellpadding="0"> <tbody> <tr> -->

<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>Task 2 Variant-1</div> </td> -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: -->
<!-- center;font-size:12px'>Task 2 Variant-2</div> </td>  -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>Task 2 -->
<!-- Variant-3 (<b>Test</b>)</div> </td> -->
<!-- </tr> -->
<!-- <tr> -->
<!-- <td align="center" valign="middle"> <div -->
<!-- style='width:50%; text-align: center;font-size:12px'>The stove off, the object and the -->
<!-- pot on the table,  the drawer closed</div> </td>  -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>The stove on, the object and the pot on the table, the drawer -->
<!-- closed</div> </td>  -->
<!-- <td align="center" -->
<!-- valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>The stove -->
<!-- on, the object and the pot on the table, the drawer not closed</div> </td> -->
<!-- </tr>   -->
<!--   <tr> -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_2.png"> <img src="./src/MultitaskKitchenDomain_2.png" style="width:50%;">  </a></td> -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_3.png"> <img src="./src/MultitaskKitchenDomain_3.png" style="width:50%;">  </a></td> -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_5.png"> <img src="./src/MultitaskKitchenDomain_5.png" style="width:50%;">  </a></td> -->
<!-- </tr> -->
<!-- </tbody> -->
<!-- </table> -->

<!-- <hr> -->
<!-- <table border="0" cellspacing="10" -->
<!-- cellpadding="0"> <tbody> <tr>  -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>Task 3 Variant-1</div> </td> -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align:center;font-size:12px'>Task 3 Variant-2</div> </td>  -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align: center;font-size:12px'>Task 3 Variant-3 (<b>Test</b>)</div> </td> -->
<!-- </tr> -->
<!-- <tr> -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align:center;font-size:12px'>The stove off, the pot on the table and the object in the pot, the drawer open</div> </td>  -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align:center;font-size:12px'>The stove off, the object and the pot on the table, the drawer closed </div> </td>  -->
<!-- <td align="center" valign="middle"> <div style='width:50%; text-align:center;font-size:12px'>The stove off, the object and the pot on the table, the drawer open</div> </td> -->
<!-- </tr>   -->
<!-- <tr> -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_1.png">  <img src="./src/MultitaskKitchenDomain_1.png" style="width:50%;">  </a></td> -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_7.png"> <img src="./src/MultitaskKitchenDomain_7.png" style="width:50%;">  </a></td> -->
<!--   <td align="center" valign="middle"><a href="./src/MultitaskKitchenDomain_8.png"> <img src="./src/MultitaskKitchenDomain_8.png" style="width:50%;">  </a></td> -->
<!-- </tr> -->
<!-- </tbody> -->
<!-- </table> -->


<!-- <table border="0" cellspacing="10" cellpadding="0" align="center"> -->
<!--   <tbody><tr><td> -->
<!--   <p align="justify" width="20%">We show the qualitative execution of -->
<!--   three tasks in <b>Train (Multi)</b> (Left column) and <b>Train -->
<!--   (Single) </b>(Right column). The three rows correspond to the three -->
<!--   tasks respectively. Skills extracted from multi-task demonstrations -->
<!--   benefit the policy learning process.</p> -->
<!-- </td></tr> -->
<!-- </tbody> -->
<!-- </table> -->

<!-- <table border="0" cellspacing="0" cellpadding="0" align="center"> -->
<!--   <tbody> -->
<!--   <tr><p></p></tr> -->
<!-- <tr> -->
<!--   <td align="center" valign="middle"> <a href="./video/task_1_BUDS.gif"> <img src="./video/task_1_BUDS.gif" style="width:50%;"> </a></td> -->
<!--   <td align="center" valign="middle"> <a href="./video/task_1_baseline.gif"> <img src="./video/task_1_baseline.gif" style="width:50%;"> </a></td> -->
<!--   </tr> -->

<!-- <tr> -->
<!--   <td align="center" valign="middle"> <a href="./video/task_2_BUDS.gif"> <img src="./video/task_2_BUDS.gif" style="width:50%;"> </a></td> -->
<!--   <td align="center" valign="middle"> <a href="./video/task_2_baseline.gif"> <img src="./video/task_2_baseline.gif" style="width:50%;"> </a></td> -->
<!--   </tr> -->

<!-- <tr> -->
<!--   <td align="center" valign="middle"> <a href="./video/task_3_BUDS.gif"> <img src="./video/task_3_BUDS.gif" style="width:50%;"> </a></td> -->
<!--   <td align="center" valign="middle"> <a href="./video/task_3_baseline.gif"> <img src="./video/task_3_baseline.gif" style="width:50%;"> </a></td> -->
<!--   </tr> -->

<!-- </tbody> -->
<!-- </table> -->


<!-- <hr> -->
<!-- <h1 align="center">Reusable Skills in <TT>Multitask-Kitchen</TT> -->
<!-- Domain</h1> -->
<!-- <table border="0" cellspacing="10" -->
<!-- cellpadding="0"><tr><td> -->
<!-- <p align="justify" width="20%">We use pie charts to show the percentage of the 8 discovered skills in each of the <tt>Multitask-Kitchen</tt> tasks (We omit the number in the figure for clarity). Most of the skills are indeed shared and reused across different tasks. And we also visualize sequences of two skills across all three tasks in the figure. As we can see from the visualization, similar skills with slightly different visual features (closing the drawer, but the stove is either on or off) are clustered in one skill, and it can improve the robustness of learned skills to visual variance in the inputs. -->
<!-- </p></td></tr></table><table border="0" cellspacing="10" cellpadding="0" align="center">  <tbody> -->
<!-- <tr> -->
<!-- 	<td align="center" valign="middle"><a href="./src/Skill_Percentage.png"> <img src="./src/Skill_Percentage.png" style="width:100%;">  </a></td> -->
<!--   </tr> -->
<!-- </tbody> -->
<!-- </table> -->


<!-- <br><br><hr> -->
<!-- <h1 align="center">Visualization of Temporal Segments</h1> -->

<!-- <table border="0" cellspacing="10" cellpadding="0" align="center"> -->
<!--   <tbody> -->
<!-- <tr> -->
<!--   <td align="center" valign="middle"><a href="./src/segmentation-real.png"> <img src="./src/segmentation-real.png" style="width:100%;">  </a></td> -->
<!--   </tr> -->
<!-- </tbody> -->
<!-- </table> -->
<!-- <table border="0" cellspacing="10" -->
<!-- cellpadding="0"><tr><td> -->
<!-- <p align="justify" width="20%">This is a visualization of temporal segments in two demonstrations -->
<!--   of <tt>Real-Kitchen</tt> with different lengths. Each cuboid corresponds to a temporal segment, and each color represents one skill that the temporal segment is clustered into. Text annotations are our interpretations of the segmented skills. We show that the temporal segments, though discovered without supervision, nicely capture semantically meaningful subtasks. They are consistent across demonstrations despite the differences in motions, e.g., the states of the tool during pushing are very different from each other. -->
<!--   </p></td></tr></table> -->



<!-- <hr> -->
<!-- <h1 align="center">Qualitative Results</h1> -->
<!-- <h2 align="center">(click to view full resolution)</h2> -->
<!-- <p> -->
<!--   </p><table border="0" cellspacing="10" cellpadding="0"> -->
<!--   <tbody> -->
<!--   <tr><td><a> gif </a></td></tr> -->
<!--   <tr><td><a> gif </a></td></tr> -->
<!--   <tr><td><a> gif </a></td></tr> -->
<!--   <tr><td><a> gif </a></td></tr> -->
<!--   <tr><td><a> gif </a></td></tr> -->
<!-- </tbody> -->
<!-- </table> -->

<!-- <hr> -->
<!-- <h1 align="center">Quantitative Results</h1> -->
<!-- <p> -->
<!--   </p><table border="0" cellspacing="10" cellpadding="0"> -->
<!--   <tbody> -->
<!--   <tr><td><h2 align="center">Description</h2></td></tr> -->
<!--   <tr><td><a>Image / Table </a></td></tr> -->
<!-- </tbody> -->
<!-- </table> -->


<!-- <hr> -->
<!-- <h1 align="center">Ablation Study</h1> -->
<!-- <h2 align="center">Example</h2> -->
<!-- <p> -->
<!--   </p><table border="0" cellspacing="10" cellpadding="0"> -->
<!--   <tbody> -->
<!--   <tr><td>PLACEHOLDER</td></tr> -->
<!--   <tr><td>PLACEHOLDER</td></tr> -->
<!-- </tbody> -->
<!-- </table> -->

<!-- <br> -->
<!-- <h2 align="center">Another examples</h2> -->
<!-- <table border="0" cellspacing="10" cellpadding="0"> -->
<!--   <tbody> -->
<!--   <tr><td>PLACEHOLDER</td></tr> -->
<!--   <tr><td>PLACEHOLDER</td></tr> -->
<!-- </tbody> -->
<!-- </table> -->

<!-- <hr> -->



<!-- <h1 align="center">Citation</h1> -->
<!--   <table align=center width=800px> -->
<!--   <tr> -->
<!--         <pre style="width:70%; font-size:10px; text-align:center"><code style="display:block; white-space:pre-wrap;text-align:left;margin-left:5%"> -->
<!-- @article{jiang2021synergies, -->
<!--   title={Synergies Between Affordance and Geometry: 6-DoF Grasp Detection via Implicit Representations}, -->
<!--   author={Jiang, Zhenyu and Zhu, Yifeng and Svetlik, Maxwell and Fang, Kuan and Zhu, Yuke}, -->
<!--   journal={arXiv preprint arXiv:2104.01542}, -->
<!--   year={2021} -->
<!-- } -->
<!--         </code></pre> -->
<!-- </tr> -->
<!-- </table> -->


<br><hr> <table align=center width=800px> <tr> <td> <left>
<center><h1>Acknowledgements</h1></center> This work has taken place
in the Robot Perception and Learning Group (RPL) and Learning Agents
Research Group (LARG) at UT Austin.  RPL research has been partially
supported by NSF CNS-1955523, the MLL Research Award from the Machine
Learning Laboratory at UT-Austin, and the Amazon Research Awards. LARG
research is supported in part by NSF (CPS-1739964, IIS-1724157,
NRI-1925082), ONR (N00014-18-2243), FLI (RFP2-000), ARO
(W911NF-19-2-0333), DARPA, Lockheed Martin, GM, and Bosch. Peter Stone
serves as the Executive Director of Sony AI America and receives
financial compensation for this work. The terms of this arrangement
have been reviewed and approved by the University of Texas at Austin
in accordance with its policy on objectivity in research.
				
<!-- The webpage template was borrowed from some <a href="https://nvlabs.github.io/SPADE/">GAN folks</a>. -->
</left></td></tr></table>
<br><br>

<div style="display:none">
<!-- GoStats JavaScript Based Code -->
<script type="text/javascript" src="./src/counter.js"></script>
<script type="text/javascript">_gos='c3.gostats.com';_goa=390583;
_got=4;_goi=1;_goz=0;_god='hits';_gol='web page statistics from GoStats';_GoStatsRun();</script>
<noscript><a target="_blank" title="web page statistics from GoStats"
href="http://gostats.com"><img alt="web page statistics from GoStats"
src="http://c3.gostats.com/bin/count/a_390583/t_4/i_1/z_0/show_hits/counter.png"
style="border-width:0" /></a></noscript>
</div>
<!-- End GoStats JavaScript Based Code -->
<!-- </center></div></body></div> -->

