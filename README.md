JS解析URL各部分通用方法
footer 固定底部        https://css-tricks.com/snippets/css/sticky-footer/

<div class="page-wrap">
  
  Content!
      
</div>

<footer class="site-footer">
  I'm the Sticky Footer.
</footer>

* {
  margin: 0;
}
html, body {
  height: 100%;
}
.page-wrap {
  min-height: 100%;
  /* equal to footer height */
  margin-bottom: -142px; 
}
.page-wrap:after {
  content: "";
  display: block;
}
.site-footer, .page-wrap:after {
  height: 142px; 
}
.site-footer {
  background: orange;
}
