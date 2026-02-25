<!DOCTYPE html>
<html>
<head>
<title>CodeMaster - Advanced Programming Portal</title>

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Segoe UI',sans-serif;}
body{background:linear-gradient(135deg,#0f2027,#203a43,#2c5364);color:white;}
header{text-align:center;padding:30px;background:rgba(255,255,255,0.05);}
header h1{font-size:2.3rem;}

.main-nav{display:flex;justify-content:center;gap:15px;padding:15px;flex-wrap:wrap;}
.main-nav button{
padding:8px 18px;border:none;border-radius:20px;
background:rgba(255,255,255,0.1);color:white;
cursor:pointer;transition:0.3s;
}
.main-nav button:hover{background:#00c6ff;transform:scale(1.1);}

.section{display:none;padding:40px;}
.section.active{display:block;}

.sub-nav{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:20px;}
.sub-nav button{
padding:6px 12px;border:none;border-radius:15px;
background:#1e3c72;color:white;cursor:pointer;
}
.sub-nav button:hover{background:#00c6ff;}

.inner-page{display:none;}
.inner-page.active{display:block;}

.card{
background:rgba(255,255,255,0.05);
padding:25px;border-radius:15px;
max-width:1100px;margin:auto;
}

.back-btn{
margin-bottom:20px;padding:6px 14px;
background:#00c6ff;border:none;border-radius:15px;cursor:pointer;
}

pre{
background:black;padding:15px;border-radius:10px;
overflow:auto;color:#00ffcc;
}

footer{text-align:center;padding:20px;background:rgba(0,0,0,0.4);}
</style>
</head>

<body>

<header>
<h1>🚀 CodeMaster Programming Hub</h1>
<p>Professional Structured Documentation</p>
</header>

<div class="main-nav">
<button onclick="showSection('home')">Home</button>
<button onclick="showSection('java')">Java</button>
<button onclick="showSection('c')">C</button>
<button onclick="showSection('cpp')">C++</button>
</div>

<!-- HOME -->
<div id="home" class="section active">
<div class="card">
<h2>Welcome Developer 👨‍💻</h2>
<p>This portal provides detailed documentation of Java, C, and C++.</p>
</div>
</div>

<!-- ================= JAVA ================= -->
<div id="java" class="section">
<div class="sub-nav">
<button onclick="openInner('java','joverview')">Overview</button>
<button onclick="openInner('java','jhistory')">History</button>
<button onclick="openInner('java','jvariables')">Variables</button>
<button onclick="openInner('java','jdatatypes')">Data Types</button>
<button onclick="openInner('java','jmethods')">Methods</button>
<button onclick="openInner('java','joop')">OOP</button>
<button onclick="openInner('java','jconstructor')">Constructor</button>
<button onclick="openInner('java','jexception')">Exception</button>
<button onclick="openInner('java','jcollections')">Collections</button>
<button onclick="openInner('java','jthread')">Multithreading</button>
</div>

<div id="joverview" class="card inner-page active">
<h2>Java Overview</h2>
<p>High-level, object-oriented, platform-independent language.</p>
<pre>
public class Main{
 public static void main(String[] args){
  System.out.println("Hello Java");
 }
}
</pre>
</div>

<div id="jhistory" class="card inner-page">
<button class="back-btn" onclick="resetInner('java','joverview')">⬅ Back</button>
<h2>History</h2>
<p>Developed by James Gosling in 1995.</p>
</div>

<div id="jvariables" class="card inner-page">
<button class="back-btn" onclick="resetInner('java','joverview')">⬅ Back</button>
<h2>Variables</h2>
<p>Local, Instance, Static, Final.</p>
</div>

<div id="jdatatypes" class="card inner-page">
<button class="back-btn" onclick="resetInner('java','joverview')">⬅ Back</button>
<h2>Data Types</h2>
<p>Primitive: int, float, double, char, boolean.</p>
<p>Non-Primitive: String, Arrays, Classes.</p>
</div>

<div id="jmethods" class="card inner-page">
<button class="back-btn" onclick="resetInner('java','joverview')">⬅ Back</button>
<h2>Methods</h2>
<pre>
int add(int a,int b){
 return a+b;
}
</pre>
</div>

<div id="joop" class="card inner-page">
<button class="back-btn" onclick="resetInner('java','joverview')">⬅ Back</button>
<h2>OOP Concepts</h2>
<p>Encapsulation, Inheritance, Polymorphism, Abstraction.</p>
</div>

<div id="jconstructor" class="card inner-page">
<button class="back-btn" onclick="resetInner('java','joverview')">⬅ Back</button>
<h2>Constructor</h2>
<pre>
class Student{
 Student(){
  System.out.println("Created");
 }
}
</pre>
</div>

<div id="jexception" class="card inner-page">
<button class="back-btn" onclick="resetInner('java','joverview')">⬅ Back</button>
<h2>Exception Handling</h2>
<pre>
try{
 int a=10/0;
}catch(Exception e){}
</pre>
</div>

<div id="jcollections" class="card inner-page">
<button class="back-btn" onclick="resetInner('java','joverview')">⬅ Back</button>
<h2>Collections</h2>
<p>ArrayList, HashMap, HashSet.</p>
</div>

<div id="jthread" class="card inner-page">
<button class="back-btn" onclick="resetInner('java','joverview')">⬅ Back</button>
<h2>Multithreading</h2>
<pre>
class A extends Thread{
 public void run(){}
}
</pre>
</div>
</div>

<!-- ================= C ================= -->
<div id="c" class="section">
<div class="sub-nav">
<button onclick="openInner('c','coverview')">Overview</button>
<button onclick="openInner('c','chistory')">History</button>
<button onclick="openInner('c','cvariables')">Variables</button>
<button onclick="openInner('c','cdatatypes')">Data Types</button>
<button onclick="openInner('c','coperators')">Operators</button>
<button onclick="openInner('c','ccontrol')">Control</button>
<button onclick="openInner('c','cfunctions')">Functions</button>
<button onclick="openInner('c','cpointers')">Pointers</button>
<button onclick="openInner('c','carrays')">Arrays</button>
<button onclick="openInner('c','cstructures')">Structures</button>
<button onclick="openInner('c','cfile')">File</button>
</div>

<div id="coverview" class="card inner-page active">
<h2>C Overview</h2>
<p>Procedural language developed in 1972.</p>
</div>

<div id="chistory" class="card inner-page">
<button class="back-btn" onclick="resetInner('c','coverview')">⬅ Back</button>
<h2>History</h2>
<p>Developed by Dennis Ritchie at Bell Labs.</p>
</div>

<div id="cvariables" class="card inner-page">
<button class="back-btn" onclick="resetInner('c','coverview')">⬅ Back</button>
<h2>Variables</h2>
<pre>
int a=10;
float b=5.5;
</pre>
</div>

<div id="cdatatypes" class="card inner-page">
<button class="back-btn" onclick="resetInner('c','coverview')">⬅ Back</button>
<h2>Data Types</h2>
<p>int, float, double, char.</p>
</div>

<div id="coperators" class="card inner-page">
<button class="back-btn" onclick="resetInner('c','coverview')">⬅ Back</button>
<h2>Operators</h2>
<p>Arithmetic, Logical, Relational.</p>
</div>

<div id="ccontrol" class="card inner-page">
<button class="back-btn" onclick="resetInner('c','coverview')">⬅ Back</button>
<h2>Control Statements</h2>
<p>if, switch, for, while, do-while.</p>
</div>

<div id="cfunctions" class="card inner-page">
<button class="back-btn" onclick="resetInner('c','coverview')">⬅ Back</button>
<h2>Functions</h2>
<pre>
int add(int a,int b){
 return a+b;
}
</pre>
</div>

<div id="cpointers" class="card inner-page">
<button class="back-btn" onclick="resetInner('c','coverview')">⬅ Back</button>
<h2>Pointers</h2>
<pre>
int x=5;
int *p=&x;
</pre>
</div>

<div id="carrays" class="card inner-page">
<button class="back-btn" onclick="resetInner('c','coverview')">⬅ Back</button>
<h2>Arrays</h2>
<pre>
int arr[5];
</pre>
</div>

<div id="cstructures" class="card inner-page">
<button class="back-btn" onclick="resetInner('c','coverview')">⬅ Back</button>
<h2>Structures</h2>
<pre>
struct Student{
 char name[20];
 int age;
};
</pre>
</div>

<div id="cfile" class="card inner-page">
<button class="back-btn" onclick="resetInner('c','coverview')">⬅ Back</button>
<h2>File Handling</h2>
<pre>
FILE *fp=fopen("data.txt","r");
</pre>
</div>
</div>

<!-- ================= C++ ================= -->
<div id="cpp" class="section">
<div class="sub-nav">
<button onclick="openInner('cpp','cppoverview')">Overview</button>
<button onclick="openInner('cpp','cpphistory')">History</button>
<button onclick="openInner('cpp','cppoop')">OOP</button>
<button onclick="openInner('cpp','cppconstructor')">Constructor</button>
<button onclick="openInner('cpp','cppdestructor')">Destructor</button>
<button onclick="openInner('cpp','cppinherit')">Inheritance</button>
<button onclick="openInner('cpp','cpppoly')">Polymorphism</button>
<button onclick="openInner('cpp','cppstl')">STL</button>
<button onclick="openInner('cpp','cppfile')">File</button>
</div>

<div id="cppoverview" class="card inner-page active">
<h2>C++ Overview</h2>
<p>Extension of C supporting OOP.</p>
</div>

<div id="cpphistory" class="card inner-page">
<button class="back-btn" onclick="resetInner('cpp','cppoverview')">⬅ Back</button>
<h2>History</h2>
<p>Developed by Bjarne Stroustrup in 1985.</p>
</div>

<div id="cppoop" class="card inner-page">
<button class="back-btn" onclick="resetInner('cpp','cppoverview')">⬅ Back</button>
<h2>OOP</h2>
<pre>
class A{};
</pre>
</div>

<div id="cppconstructor" class="card inner-page">
<button class="back-btn" onclick="resetInner('cpp','cppoverview')">⬅ Back</button>
<h2>Constructor</h2>
<pre>
class A{ public: A(){} };
</pre>
</div>

<div id="cppdestructor" class="card inner-page">
<button class="back-btn" onclick="resetInner('cpp','cppoverview')">⬅ Back</button>
<h2>Destructor</h2>
<pre>
~A(){}
</pre>
</div>

<div id="cppinherit" class="card inner-page">
<button class="back-btn" onclick="resetInner('cpp','cppoverview')">⬅ Back</button>
<h2>Inheritance</h2>
<pre>
class B: public A{};
</pre>
</div>

<div id="cpppoly" class="card inner-page">
<button class="back-btn" onclick="resetInner('cpp','cppoverview')">⬅ Back</button>
<h2>Polymorphism</h2>
<p>Function Overloading and Virtual Functions.</p>
</div>

<div id="cppstl" class="card inner-page">
<button class="back-btn" onclick="resetInner('cpp','cppoverview')">⬅ Back</button>
<h2>STL</h2>
<p>vector, map, set, list.</p>
</div>

<div id="cppfile" class="card inner-page">
<button class="back-btn" onclick="resetInner('cpp','cppoverview')">⬅ Back</button>
<h2>File Handling</h2>
<pre>
fstream file;
file.open("data.txt");
</pre>
</div>

</div>

<footer>
© 2026 CodeMaster | Advanced Documentation
</footer>

<script>
function showSection(id){
document.querySelectorAll('.section').forEach(s=>s.classList.remove('active'));
document.getElementById(id).classList.add('active');
}
function openInner(section,id){
document.querySelectorAll('#'+section+' .inner-page')
.forEach(p=>p.classList.remove('active'));
document.getElementById(id).classList.add('active');
}
function resetInner(section,defaultId){
document.querySelectorAll('#'+section+' .inner-page')
.forEach(p=>p.classList.remove('active'));
document.getElementById(defaultId).classList.add('active');
}
</script>

</body>
</html>
