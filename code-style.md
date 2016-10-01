 <h3 class="doc-title">
   
 <h3>一、缩进、空格规范</h3>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E7%BC%A9%E8%BF%9B" rel="nofollow"></a>缩进：</h5><p>一个代码块与上一级的代码快之间使用四个空格来进行缩进</p><p>注意使用四个空格而非一个tab来进行缩进</p><p>文件中不允许在任何地方使用tab</p><h5>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E5%A4%A7%E6%8B%AC%E5%8F%B7" rel="nofollow"></a>大括号：</h5><p>前一个大括号写到后面并与之前的代码相隔一个空格而非另起一行写</p><p>后一个大括号独占一行并与相应的代码块对齐</p><p>(有点绕口，等下看后面的例子就一下明白了)</p><h5>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E7%A9%BA%E6%A0%BC" rel="nofollow"></a>空格：</h5><ol>
<li>
<p>方法的参数</p>
<p>方法如果有多个参数, 写完一个参数的逗号之后应当有一个空格</p>
<p>例如：</p>
<pre><code>public void fuckThisWorld(String tools, int time, bool isFull) {
    (省略了函数体)
}
</code></pre>
<p>注意方法的三个参数之间的两个逗号后都有个空格，参数和小括号之间没有空格</p>
</li>
<li>
<p>for循环</p>
<p>用一个例子来说明：</p>
<pre><code>for(int i=0; i &lt; 100; i++) {
    (省略了循环体)
}
</code></pre>
<p>注意每个分号之后有一个空格</p>
</li>
<li>
<p>运算符</p>
<p>比较运算符、逻辑运算符、算数运算符前后要有一个空格</p>
</li>
</ol><h5>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E8%A7%84%E8%8C%83%E7%9A%84%E4%BE%8B%E5%AD%90" rel="nofollow"></a>规范的例子：</h5><pre><code class="lang-java">public class Example {
    public static void firstExample(int size, int ass) {
        for(int i=0; i &lt; size; i++) {
            if(i == 999) {
                break;
            }
        }
    }
}
</code></pre><hr><h3>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E4%BA%8C%E5%91%BD%E5%90%8D%E8%A7%84%E8%8C%83" rel="nofollow"></a>二、命名规范</h3><h5>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E9%80%9A%E7%94%A8%E8%A7%84%E5%88%99" rel="nofollow"></a>通用规则：</h5><ol>
<li>
<p>原则：</p>
<p>命名应当达到“见其名知其意”</p>
<p>一个类、方法、变量等等的命名应当使得阅读代码的人能够通过它的名字来判断出它的意思和作用</p>
<p>例如：</p>
<pre><code>int asshole;    //可以的变量名，通过名字就可以知道这个变量的意思
int a;          //不好的名字，谁知道a代表什么东西
</code></pre>
</li>
<li>
<p>缩写：</p>
<p>首先尽量少用缩写</p>
<p>如果在命名中使用缩写，</p>
<p>请使用一些广为人知的缩写，不要使用大部分人不知道，你自己自创的缩写</p>
<p>不要使用一些可能引起歧义的缩写</p>
<p>例如：</p>
<pre><code>int num;    //好缩写，num代表number是广为人知的
int pc;     //不好的缩写，因为pc可能代表的意思太多了
int n;      //不好的缩写，不明其义
</code></pre>
</li>
</ol><h5>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E7%B1%BB%E5%91%BD%E5%90%8D" rel="nofollow"></a>类命名：</h5><p>使用大驼峰命名法，每一个单词的首字母大写，其余字母小写。</p><p>例如:</p><pre><code>TextView, EditText, PornVideo都是规范的类命名
textView, textview, text_view都是不规范的类命名
</code></pre><h5>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E6%96%B9%E6%B3%95%E5%91%BD%E5%90%8D" rel="nofollow"></a>方法命名：</h5><p>使用小驼峰命名法，即变量第一个单词的首字母小写，其余单词的首字母大写</p><p>例如：</p><pre><code>getInstance, fuckDog, addChild都是规范的方法命名
GetInstance, getinstance, get_instance都是不规范的方法命名
</code></pre><h5>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E5%8F%98%E9%87%8F%E5%91%BD%E5%90%8D" rel="nofollow"></a>变量命名：</h5><p>对于常量，使用大写字母加下划线的方法来进行命名</p><p>例如：</p><pre><code>final private static String ONE_NIGHT_SEX_LOCATION="DongGuan";
</code></pre><p>对于其余的变量，使用小驼峰命名法</p><p>例如：</p><pre><code class="lang-java">int isFucked;
Thread netThread;
</code></pre><hr><h3>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E4%B8%89%E6%B3%A8%E9%87%8A%E8%A7%84%E8%8C%83" rel="nofollow"></a>三、注释规范</h3><p>参考javadoc注释规范</p><h5>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E5%87%BD%E6%95%B0%E6%B3%A8%E9%87%8A" rel="nofollow"></a>函数注释:</h5><p>例子：</p><pre><code>/**
 * 将ip地址的整数类型转化为字符串
 * @param ipInt IP地址的整数类型
 * @return IP地址的字符串格式
 */
private static String formatIp(int ipInt) {
    return (ipInt &amp; 0xFF) + "." + ((ipInt &gt;&gt; 8) &amp; 0xFF) + "." + ((ipInt &gt;&gt; 16) &amp; 0xFF) + "." + ((ipInt &gt;&gt; 24) &amp; 0xFF);
}
</code></pre><p>如上例，对于每一个函数，需要对首先说明这个函数的大致作用，之后还要说明这个函数的每个参数以及返回值</p><p>如果函数过于简单，通过名称就可以十分准确地推断出这个函数的返回值、参数、函数作用的话，可以不加以注释</p><h5>
<a href="https://github.com/fallenworld/AndroidTask/blob/master/CodeSpecification.md#%E4%BB%A3%E7%A0%81%E5%AE%9E%E7%8E%B0%E6%B3%A8%E9%87%8A" rel="nofollow"></a>代码实现注释：</h5><p>代码实现中的注释要求一个原则：只在需要的地方注释，注释不宜过多</p><p>代码实现中的注释使用单行两个斜杠//来进行注释</p><p>注释应当写到被注释代码的上一行</p>
    </div>