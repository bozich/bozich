# Все про С++ из сайта ravesli.com

Сдесь я собрал всю информацию про С++ (на 2021 год) из онлайн-учебника ravesli. Цель: удобство, а также [pdf файл](http://github.com/bozich/bozich/raw/master/articles/ravesli-cpp/index.pdf) в репозитории [GitHub](http://github.com/bozich/bozich/tree/master/articles/ravesli-cpp/)

Веб-Сайт автора: [bozich.github.io](http://bozich.github.io).

Что-ж, начнем!

# Урок №1. Введение в программирование

<div class="sam-content">




<h1 class="zagolovokstat">Урок №1. Введение в программирование</h1>
	
<!-- Go to www.addthis.com/dashboard to customize your tools -->
<script type="text/javascript" src="//s7.addthis.com/js/300/addthis_widget.js#pubid=ra-5e19d0f6e5c76fb3"></script>
<!-- Go to www.addthis.com/dashboard to customize your tools -->
<div class="addthis_inline_share_toolbox" data-url="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/" data-title="Введение в программирование | Уроки С++ - Ravesli" data-description="Компьютеры понимают только очень ограниченный набор инструкций, и чтобы заставить их что-то делать, нужно четко сформулировать задание, используя эти же инструкции. Программа (также «приложение» или «программное обеспечение», или «софт») - это набор инструкций, которые указывают компьютеру, что ему нужно делать. Физическая часть компьютера, которая выполняет эти инструкции, называется «железом» или аппаратной частью (например, процессор, материнская плата и т.д.). Данный урок является началом серии уроков по программированию на языке С++ для начинающих." style="clear: both;"><div id="atstbx2" class="at-resp-share-element at-style-responsive addthis-smartlayers addthis-animated at4-show" aria-labelledby="at-cf7440d8-173d-4da7-902c-923d0413f007" role="region"><span id="at-cf7440d8-173d-4da7-902c-923d0413f007" class="at4-visually-hidden">AddThis Sharing Buttons</span><div class="at-share-btn-elements"><a role="button" tabindex="0" class="at-icon-wrapper at-share-btn at-svc-vk" style="background-color: rgb(99, 131, 168); border-radius: 0px;"><span class="at4-visually-hidden">Share to Vkontakte</span><span class="at-icon-wrapper" style="line-height: 32px; height: 32px; width: 32px;"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 32 32" version="1.1" role="img" aria-labelledby="at-svg-vk-1" class="at-icon at-icon-vk" style="fill: rgb(255, 255, 255); width: 32px; height: 32px;"><title id="at-svg-vk-1">Vkontakte</title><g><path d="M26.712 10.96s-.167-.48-1.21-.348l-3.447.024a.785.785 0 0 0-.455.072s-.204.108-.3.37a22.1 22.1 0 0 1-1.28 2.695c-1.533 2.61-2.156 2.754-2.407 2.587-.587-.372-.43-1.51-.43-2.323 0-2.54.382-3.592-.756-3.868-.37-.084-.646-.144-1.616-.156-1.232-.012-2.274 0-2.86.287-.396.193-.695.624-.515.648.227.036.742.143 1.017.515 0 0 .3.49.347 1.568.13 2.982-.48 3.353-.48 3.353-.466.252-1.28-.167-2.478-2.634 0 0-.694-1.222-1.233-2.563-.097-.25-.288-.383-.288-.383s-.216-.168-.527-.216l-3.28.024c-.504 0-.683.228-.683.228s-.18.19-.012.587c2.562 6.022 5.483 9.04 5.483 9.04s2.67 2.79 5.7 2.597h1.376c.418-.035.634-.263.634-.263s.192-.214.18-.61c-.024-1.843.838-2.12.838-2.12.838-.262 1.915 1.785 3.065 2.575 0 0 .874.6 1.532.467l3.064-.048c1.617-.01.85-1.352.85-1.352-.06-.108-.442-.934-2.286-2.647-1.916-1.784-1.665-1.496.658-4.585 1.413-1.88 1.976-3.03 1.796-3.52z" fill-rule="evenodd"></path></g></svg></span><span class="at-label" style="font-size: 11.4px; line-height: 32px; height: 32px; color: rgb(255, 255, 255);">Vkontakte</span></a><a role="button" tabindex="0" class="at-icon-wrapper at-share-btn at-svc-telegram" style="background-color: rgb(0, 136, 204); border-radius: 0px;"><span class="at4-visually-hidden">Share to Telegram</span><span class="at-icon-wrapper" style="line-height: 32px; height: 32px; width: 32px;"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 32 32" version="1.1" role="img" aria-labelledby="at-svg-telegram-2" class="at-icon at-icon-telegram" style="fill: rgb(255, 255, 255); width: 32px; height: 32px;"><title id="at-svg-telegram-2">Telegram</title><g><g fill-rule="evenodd"></g><path d="M15.02 20.814l9.31-12.48L9.554 17.24l1.92 6.42c.225.63.114.88.767.88l.344-5.22 2.436 1.494z" opacity=".6"></path><path d="M12.24 24.54c.504 0 .727-.234 1.008-.51l2.687-2.655-3.35-2.054-.344 5.22z" opacity=".3"></path><path d="M12.583 19.322l8.12 6.095c.926.52 1.595.25 1.826-.874l3.304-15.825c.338-1.378-.517-2.003-1.403-1.594L5.024 14.727c-1.325.54-1.317 1.29-.24 1.625l4.98 1.58 11.53-7.39c.543-.336 1.043-.156.633.214"></path></g></svg></span><span class="at-label" style="font-size: 11.4px; line-height: 32px; height: 32px; color: rgb(255, 255, 255);">Telegram</span></a><a role="button" tabindex="0" class="at-icon-wrapper at-share-btn at-svc-facebook" style="background-color: rgb(59, 89, 152); border-radius: 0px;"><span class="at4-visually-hidden">Share to Facebook</span><span class="at-icon-wrapper" style="line-height: 32px; height: 32px; width: 32px;"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 32 32" version="1.1" role="img" aria-labelledby="at-svg-facebook-3" class="at-icon at-icon-facebook" style="fill: rgb(255, 255, 255); width: 32px; height: 32px;"><title id="at-svg-facebook-3">Facebook</title><g><path d="M22 5.16c-.406-.054-1.806-.16-3.43-.16-3.4 0-5.733 1.825-5.733 5.17v2.882H9v3.913h3.837V27h4.604V16.965h3.823l.587-3.913h-4.41v-2.5c0-1.123.347-1.903 2.198-1.903H22V5.16z" fill-rule="evenodd"></path></g></svg></span><span class="at-label" style="font-size: 11.4px; line-height: 32px; height: 32px; color: rgb(255, 255, 255);">Facebook</span></a><a role="button" tabindex="0" class="at-icon-wrapper at-share-btn at-svc-twitter" style="background-color: rgb(29, 161, 242); border-radius: 0px;"><span class="at4-visually-hidden">Share to Twitter</span><span class="at-icon-wrapper" style="line-height: 32px; height: 32px; width: 32px;"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 32 32" version="1.1" role="img" aria-labelledby="at-svg-twitter-4" class="at-icon at-icon-twitter" style="fill: rgb(255, 255, 255); width: 32px; height: 32px;"><title id="at-svg-twitter-4">Twitter</title><g><path d="M27.996 10.116c-.81.36-1.68.602-2.592.71a4.526 4.526 0 0 0 1.984-2.496 9.037 9.037 0 0 1-2.866 1.095 4.513 4.513 0 0 0-7.69 4.116 12.81 12.81 0 0 1-9.3-4.715 4.49 4.49 0 0 0-.612 2.27 4.51 4.51 0 0 0 2.008 3.755 4.495 4.495 0 0 1-2.044-.564v.057a4.515 4.515 0 0 0 3.62 4.425 4.52 4.52 0 0 1-2.04.077 4.517 4.517 0 0 0 4.217 3.134 9.055 9.055 0 0 1-5.604 1.93A9.18 9.18 0 0 1 6 23.85a12.773 12.773 0 0 0 6.918 2.027c8.3 0 12.84-6.876 12.84-12.84 0-.195-.005-.39-.014-.583a9.172 9.172 0 0 0 2.252-2.336" fill-rule="evenodd"></path></g></svg></span><span class="at-label" style="font-size: 11.4px; line-height: 32px; height: 32px; color: rgb(255, 255, 255);">Twitter</span></a></div></div></div>
	
<p class="data" style="float: none; line-height: 15px; margin-top: 25px;"><i class="fa fa-user">&nbsp;&nbsp;</i><a href="https://ravesli.com/author/yura_ravesli/" class="data" style="float: none; line-height: 15px;" target="_blank">Юрий</a>&nbsp;&nbsp;|&nbsp;</p>
	
	<div class="catsingle"><ul class="post-categories">
	<li><a href="https://ravesli.com/category/uroki-s/" rel="category tag">Уроки С++</a></li></ul>&nbsp;&nbsp;|&nbsp;</div>


<p class="data" style="float: none; line-height: 15px;"><i class="fas fa-pen-nib"></i>&nbsp;&nbsp;Обновл. 24 Дек 2020&nbsp;&nbsp;|&nbsp;</p>

	
	

	
	<div class="catsingle" style="padding-bottom: 20px;"><i class="fa fa-eye" aria-hidden="true"></i>&nbsp;211115 </div>

		<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comments"><p class="data" style="float: none;">&nbsp;ǀ&nbsp;&nbsp;<i class="fa fa-comments"></i>&nbsp;55&nbsp;</p></a>


	
<div class="content">
<p>Компьютеры понимают только очень ограниченный набор инструкций, и чтобы заставить их что-то делать, нужно четко сформулировать задание, используя эти же инструкции. <strong>Программа</strong> (также «<em>приложение</em>» или «<em>программное обеспечение</em>», или «<em>софт</em>») — это набор инструкций, которые указывают компьютеру, что ему нужно делать. Физическая часть компьютера, которая выполняет эти инструкции, называется&nbsp;<strong><em>«железом»</em></strong> или&nbsp;<em><strong>аппаратной частью</strong></em> (например, процессор, материнская плата и т.д.). Данный урок является началом серии уроков по программированию на языке С++ для начинающих.</p>
<div class="toc">
<div class="czagvstat">Оглавление:</div>
<div class="toc_list">
<ol>
<li class="toc_item"><a href="#toc-0">Машинный язык</a></li>
<li class="toc_item"><a href="#toc-1">Язык ассемблера</a></li>
<li class="toc_item"><a href="#toc-2">Высокоуровневые языки программирования</a></li>
<li class="toc_item"><a href="#toc-3">Преимущества высокоуровневых языков программирования</a></li>
</ol>
</div>
</div>
<p><a style="text-decoration: none;" name="toc-0"></a></p>
<h2 class="czagvstat">Машинный язык</h2>
<p>Процессор компьютера не способен понимать напрямую языки программирования, такие как C++, Java, Python и т.д. Очень ограниченный набор инструкций, которые изначально понимает процессор, называется&nbsp;<strong>машинным кодом</strong> (или <strong><em>«машинным языком»</em></strong>). То, как эти инструкции организованы, выходит за рамки данного введения, но стоит отметить две вещи.</p>
<p>Во-первых, каждая команда (инструкция) состоит только из определенной последовательности (набора) цифр: <code style="font-size: 1.2em;">0</code> и <code style="font-size: 1.2em;">1</code>. Эти числа называются <strong>битами</strong> (сокр. от <em>«<strong>bi</strong>nary digi<strong>t</strong>»</em>) или <strong>двоичным кодом</strong>.</p>
<p>Например, одна команда машинного кода архитектуры ×86 выглядит следующим образом:</p>
<p><code style="font-size: 1.2em;">10110000 01100001</code></p>
<p>Во-вторых, каждый набор бит переводится процессором в инструкции для выполнения определенного задания (например, <em>сравнить два числа</em>&nbsp;или <em>переместить число в определенную ячейку памяти</em>). Разные типы процессоров обычно имеют разные наборы инструкций, поэтому инструкции, которые будут работать на процессорах Intel (используются в персональных компьютерах), с большей долей вероятности, не будут работать на процессорах Xenon (используются в игровых приставках Xbox). Раньше, когда компьютеры только начинали массово распространяться, программисты должны были писать программы непосредственно на машинном языке, что было очень неудобно, сложно и занимало намного больше времени, чем сейчас.<br>
<a style="text-decoration: none;" name="toc-1"></a></p>
<h2 class="czagvstat">Язык ассемблера</h2><script async="" src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle" style="display:block; text-align:center;" data-ad-layout="in-article" data-ad-format="fluid" data-ad-client="ca-pub-1157306330783763" data-ad-slot="9477964340"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script><br>
<p>Так как программировать на машинном языке — удовольствие специфическое, то программисты изобрели язык ассемблера. В этом языке каждая команда идентифицируется коротким именем (а не набором единиц с нулями), и переменными можно управлять через их имена. Таким образом, писать/читать код стало гораздо легче. Тем не менее, процессор все равно не понимает язык ассемблера напрямую. Его также нужно переводить, с помощью ассемблера, в машинный код. <strong>Ассемблер </strong>— это транслятор (переводчик), который переводит код, написанный на языке ассемблера, в машинный язык. В Интернете язык ассемблера часто называют просто <em>«Ассемблер»</em>.</p>
<p>Преимуществом Ассемблера является его производительность (точнее скорость выполнения) и он до сих пор используется, когда это имеет решающее значение. Тем не менее, причина подобного преимущества заключается в том, что программирование на этом языке адаптируется к конкретному процессору. Программы, адаптированные под один процессор, не будут работать с другим. Кроме того, чтобы программировать на Ассемблере, по-прежнему нужно знать очень много не очень читабельных инструкций для выполнения даже простого задания.</p>
<p>Например, вот вышеприведенная команда, но уже на языке ассемблера:</p>
<p><code style="font-size: 1.2em;">mov al, 061h</code><br>
<a style="text-decoration: none;" name="toc-2"></a></p>
<h2 class="czagvstat">Высокоуровневые языки программирования</h2>
<p>Для решения проблем читабельности кода и чрезмерной сложности были разработаны высокоуровневые языки программирования. C, C++, Pascal, Java, JavaScript и Perl — это всё <strong>языки высокого уровня</strong>. Они позволяют писать и выполнять программы, не переживая о совместимости кода с разными архитектурами процессоров. Программы, написанные на языках высокого уровня, также должны быть переведены в машинный код перед выполнением. Есть два варианта:</p>
<p style="padding-left: 20px;"><i class="fas fa-arrow-right fa-md"></i>&nbsp; &nbsp;компиляция, которая выполняется компилятором;</p>
<p style="padding-left: 20px;"><i class="fas fa-arrow-right fa-md"></i>&nbsp; &nbsp;интерпретация, которая выполняется интерпретатором.</p>
<p><strong>Компилятор</strong> — это программа, которая читает код и создает автономную (способную работать независимо от другого аппаратного или программного обеспечения) исполняемую программу, которую процессор понимает напрямую. При запуске программы весь код компилируется целиком, а затем создается исполняемый файл и уже при повторном запуске программы компиляция не выполняется.</p>
<p>Проще говоря, процесс компиляции выглядит следующим образом:</p>
<p><img loading="lazy" class="aligncenter size-full wp-image-4168" src="https://ravesli.com/wp-content/uploads/2016/04/sxemagotovoOk.jpg" alt="" width="625" height="185" srcset="https://ravesli.com/wp-content/uploads/2016/04/sxemagotovoOk.jpg 625w, https://ravesli.com/wp-content/uploads/2016/04/sxemagotovoOk-300x89.jpg 300w, https://ravesli.com/wp-content/uploads/2016/04/sxemagotovoOk-283x84.jpg 283w" sizes="(max-width: 625px) 100vw, 625px"></p>
<p><strong>Интерпретатор</strong> — это программа, которая напрямую выполняет код, без его предыдущей компиляции в исполняемый файл. Интерпретаторы более гибкие, но менее эффективные, так как процесс интерпретации выполняется повторно при каждом запуске программы.</p>
<p>Процесс интерпретации:<strong><em>&nbsp;</em></strong></p>
<p><img loading="lazy" class="aligncenter size-full wp-image-4169" src="https://ravesli.com/wp-content/uploads/2016/04/sxemagotovo22Ok.jpg" alt="" width="800" height="100" srcset="https://ravesli.com/wp-content/uploads/2016/04/sxemagotovo22Ok.jpg 800w, https://ravesli.com/wp-content/uploads/2016/04/sxemagotovo22Ok-300x38.jpg 300w, https://ravesli.com/wp-content/uploads/2016/04/sxemagotovo22Ok-768x96.jpg 768w, https://ravesli.com/wp-content/uploads/2016/04/sxemagotovo22Ok-283x35.jpg 283w" sizes="(max-width: 800px) 100vw, 800px"></p>
<p>Любой язык программирования может быть компилируемым или интерпретируемым, однако, такие языки, как C, C++ и Pascal — компилируются, в то время как «скриптовые» языки, такие, как Perl и JavaScript — интерпретируются. Некоторые языки программирования (например, Java) могут как компилироваться, так и интерпретироваться.<br>
<a style="text-decoration: none;" name="toc-3"></a></p>
<h2 class="czagvstat">Преимущества высокоуровневых языков программирования</h2><script async="" src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle" style="display:block; text-align:center;" data-ad-layout="in-article" data-ad-format="fluid" data-ad-client="ca-pub-1157306330783763" data-ad-slot="9477964340"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script><br>
<p><strong><em>Преимущество №1</em>:</strong> Легче писать/читать код. Вот вышеприведенная команда, но уже на языке C++:</p>
<p><code style="font-size: 1.2em;">а = 97;</code></p>
<p><strong><em>Преимущество №2:</em></strong> Требуется меньше инструкций для выполнения определенного задания. В языке C++ вы можете сделать что-то вроде <code style="font-size: 1.2em;">а = Ь * 2 + 5;</code> в одной строке. В языке ассемблера вам пришлось бы использовать 5 или 6 инструкций.</p>
<p><strong><em>Преимущество №3:</em></strong> Вы не должны заботиться о таких деталях, как загрузка переменных в регистры процессора. Компилятор или интерпретатор берёт это на себя.</p>
<p><strong><em>Преимущество №4:</em></strong> Высокоуровневые языки программирования более портируемые под различные архитектуры (но есть один нюанс).<img loading="lazy" class="aligncenter size-full wp-image-1411" src="/wp-content/uploads/2016/04/sxemagotovo33.jpg" alt="sxemagotovo33" width="650" height="300" srcset="https://ravesli.com/wp-content/uploads/2016/04/sxemagotovo33.jpg 650w, https://ravesli.com/wp-content/uploads/2016/04/sxemagotovo33-300x138.jpg 300w, https://ravesli.com/wp-content/uploads/2016/04/sxemagotovo33-283x131.jpg 283w" sizes="(max-width: 650px) 100vw, 650px">Нюанс заключается в том, что многие платформы, такие как Microsoft Windows, имеют свои собственные специфические функции, с помощью которых писать код намного легче. Но в таком случае приходится жертвовать портируемостью, так как функции, специфические для одной платформы, с большей долей вероятности, не будут работать на другой платформе. Обо всем этом мы детально поговорим на следующих уроках.</p>


<div class="ratings" style="text-align: center; margin-top: 45px;">
<p>Оценить статью:</p>
<div id="post-ratings-1377" class="post-ratings" itemscope="" itemtype="http://schema.org/Article" data-nonce="fd43077a87"><img id="rating_1377_1" src="https://ravesli.com/wp-content/plugins/wp-postratings/images/stars_crystal/rating_on.gif" alt="Звёзд: 1" title="Звёзд: 1" onmouseover="current_rating(1377, 1, 'Звёзд: 1');" onmouseout="ratings_off(4.9, 5, 0);" onclick="rate_post();" onkeypress="rate_post();" style="cursor: pointer; border: 0px;"><img id="rating_1377_2" src="https://ravesli.com/wp-content/plugins/wp-postratings/images/stars_crystal/rating_on.gif" alt="Звёзд: 2" title="Звёзд: 2" onmouseover="current_rating(1377, 2, 'Звёзд: 2');" onmouseout="ratings_off(4.9, 5, 0);" onclick="rate_post();" onkeypress="rate_post();" style="cursor: pointer; border: 0px;"><img id="rating_1377_3" src="https://ravesli.com/wp-content/plugins/wp-postratings/images/stars_crystal/rating_on.gif" alt="Звёзд: 3" title="Звёзд: 3" onmouseover="current_rating(1377, 3, 'Звёзд: 3');" onmouseout="ratings_off(4.9, 5, 0);" onclick="rate_post();" onkeypress="rate_post();" style="cursor: pointer; border: 0px;"><img id="rating_1377_4" src="https://ravesli.com/wp-content/plugins/wp-postratings/images/stars_crystal/rating_on.gif" alt="Звёзд: 4" title="Звёзд: 4" onmouseover="current_rating(1377, 4, 'Звёзд: 4');" onmouseout="ratings_off(4.9, 5, 0);" onclick="rate_post();" onkeypress="rate_post();" style="cursor: pointer; border: 0px;"><img id="rating_1377_5" src="https://ravesli.com/wp-content/plugins/wp-postratings/images/stars_crystal/rating_half.gif" alt="Звёзд: 5" title="Звёзд: 5" onmouseover="current_rating(1377, 5, 'Звёзд: 5');" onmouseout="ratings_off(4.9, 5, 0);" onclick="rate_post();" onkeypress="rate_post();" style="cursor: pointer; border: 0px;"> (<strong>2&nbsp;098</strong> оценок, среднее: <strong>4,87</strong> из 5)<br><span class="post-ratings-text" id="ratings_1377_text"></span><meta itemprop="name" content="Урок №1. Введение в программирование"><meta itemprop="headline" content="Урок №1. Введение в программирование"><meta itemprop="description" content="Компьютеры понимают только очень ограниченный набор инструкций, и чтобы заставить их что-то делать, нужно четко сформулировать задание, используя эти же инструкции. Программа (также «приложение» или «..."><meta itemprop="datePublished" content="2016-04-02T02:07:18+03:00"><meta itemprop="dateModified" content="2020-12-24T19:08:53+03:00"><meta itemprop="url" content="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/"><meta itemprop="author" content="Юрий"><meta itemprop="mainEntityOfPage" content="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/"><div style="display: none;" itemprop="image" itemscope="" itemtype="https://schema.org/ImageObject"><meta itemprop="url" content="https://ravesli.com/wp-content/uploads/2016/04/urok1-150x150.jpg"><meta itemprop="width" content="150"><meta itemprop="height" content="150"></div><div style="display: none;" itemprop="publisher" itemscope="" itemtype="https://schema.org/Organization"><meta itemprop="name" content="Ravesli"><meta itemprop="url" content="https://ravesli.com"><div itemprop="logo" itemscope="" itemtype="https://schema.org/ImageObject"><meta itemprop="url" content="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3.jpg"></div></div></div><div id="post-ratings-1377-loading" class="post-ratings-loading"><img src="https://ravesli.com/wp-content/plugins/wp-postratings/images/loading.gif" width="16" height="16" class="post-ratings-image"> Загрузка...</div>	</div>
	

	


<!-- uSocial -->
<div class="social-share-buttons">
<p class="share-text"><strong>Поделиться в социальных сетях:</strong></p>
<div style="margin-top: 20px;">
<!-- Go to www.addthis.com/dashboard to customize your tools -->
<script type="text/javascript" src="//s7.addthis.com/js/300/addthis_widget.js#pubid=ra-5e19d0f6e5c76fb3"></script>

<!-- Go to www.addthis.com/dashboard to customize your tools -->
<div class="addthis_inline_share_toolbox_hv0g" data-url="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/" data-title="Введение в программирование | Уроки С++ - Ravesli" data-description="Компьютеры понимают только очень ограниченный набор инструкций, и чтобы заставить их что-то делать, нужно четко сформулировать задание, используя эти же инструкции. Программа (также «приложение» или «программное обеспечение», или «софт») - это набор инструкций, которые указывают компьютеру, что ему нужно делать. Физическая часть компьютера, которая выполняет эти инструкции, называется «железом» или аппаратной частью (например, процессор, материнская плата и т.д.). Данный урок является началом серии уроков по программированию на языке С++ для начинающих." style="clear: both;"><div id="atstbx3" class="at-resp-share-element at-style-responsive addthis-smartlayers addthis-animated at4-show" aria-labelledby="at-8e30e482-fd0f-40b3-a56a-1aab1c774319" role="region"><span id="at-8e30e482-fd0f-40b3-a56a-1aab1c774319" class="at4-visually-hidden">AddThis Sharing Buttons</span><div class="at-share-btn-elements"><a role="button" tabindex="0" class="at-icon-wrapper at-share-btn at-svc-vk" style="background-color: rgb(99, 131, 168); border-radius: 0px;"><span class="at4-visually-hidden">Share to Vkontakte</span><span class="at-icon-wrapper" style="line-height: 32px; height: 32px; width: 32px;"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 32 32" version="1.1" role="img" aria-labelledby="at-svg-vk-5" class="at-icon at-icon-vk" style="fill: rgb(255, 255, 255); width: 32px; height: 32px;"><title id="at-svg-vk-5">Vkontakte</title><g><path d="M26.712 10.96s-.167-.48-1.21-.348l-3.447.024a.785.785 0 0 0-.455.072s-.204.108-.3.37a22.1 22.1 0 0 1-1.28 2.695c-1.533 2.61-2.156 2.754-2.407 2.587-.587-.372-.43-1.51-.43-2.323 0-2.54.382-3.592-.756-3.868-.37-.084-.646-.144-1.616-.156-1.232-.012-2.274 0-2.86.287-.396.193-.695.624-.515.648.227.036.742.143 1.017.515 0 0 .3.49.347 1.568.13 2.982-.48 3.353-.48 3.353-.466.252-1.28-.167-2.478-2.634 0 0-.694-1.222-1.233-2.563-.097-.25-.288-.383-.288-.383s-.216-.168-.527-.216l-3.28.024c-.504 0-.683.228-.683.228s-.18.19-.012.587c2.562 6.022 5.483 9.04 5.483 9.04s2.67 2.79 5.7 2.597h1.376c.418-.035.634-.263.634-.263s.192-.214.18-.61c-.024-1.843.838-2.12.838-2.12.838-.262 1.915 1.785 3.065 2.575 0 0 .874.6 1.532.467l3.064-.048c1.617-.01.85-1.352.85-1.352-.06-.108-.442-.934-2.286-2.647-1.916-1.784-1.665-1.496.658-4.585 1.413-1.88 1.976-3.03 1.796-3.52z" fill-rule="evenodd"></path></g></svg></span><span class="at-label" style="font-size: 11.4px; line-height: 32px; height: 32px; color: rgb(255, 255, 255);">Vkontakte</span></a><a role="button" tabindex="0" class="at-icon-wrapper at-share-btn at-svc-telegram" style="background-color: rgb(0, 136, 204); border-radius: 0px;"><span class="at4-visually-hidden">Share to Telegram</span><span class="at-icon-wrapper" style="line-height: 32px; height: 32px; width: 32px;"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 32 32" version="1.1" role="img" aria-labelledby="at-svg-telegram-6" class="at-icon at-icon-telegram" style="fill: rgb(255, 255, 255); width: 32px; height: 32px;"><title id="at-svg-telegram-6">Telegram</title><g><g fill-rule="evenodd"></g><path d="M15.02 20.814l9.31-12.48L9.554 17.24l1.92 6.42c.225.63.114.88.767.88l.344-5.22 2.436 1.494z" opacity=".6"></path><path d="M12.24 24.54c.504 0 .727-.234 1.008-.51l2.687-2.655-3.35-2.054-.344 5.22z" opacity=".3"></path><path d="M12.583 19.322l8.12 6.095c.926.52 1.595.25 1.826-.874l3.304-15.825c.338-1.378-.517-2.003-1.403-1.594L5.024 14.727c-1.325.54-1.317 1.29-.24 1.625l4.98 1.58 11.53-7.39c.543-.336 1.043-.156.633.214"></path></g></svg></span><span class="at-label" style="font-size: 11.4px; line-height: 32px; height: 32px; color: rgb(255, 255, 255);">Telegram</span></a><a role="button" tabindex="0" class="at-icon-wrapper at-share-btn at-svc-facebook" style="background-color: rgb(59, 89, 152); border-radius: 0px;"><span class="at4-visually-hidden">Share to Facebook</span><span class="at-icon-wrapper" style="line-height: 32px; height: 32px; width: 32px;"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 32 32" version="1.1" role="img" aria-labelledby="at-svg-facebook-7" class="at-icon at-icon-facebook" style="fill: rgb(255, 255, 255); width: 32px; height: 32px;"><title id="at-svg-facebook-7">Facebook</title><g><path d="M22 5.16c-.406-.054-1.806-.16-3.43-.16-3.4 0-5.733 1.825-5.733 5.17v2.882H9v3.913h3.837V27h4.604V16.965h3.823l.587-3.913h-4.41v-2.5c0-1.123.347-1.903 2.198-1.903H22V5.16z" fill-rule="evenodd"></path></g></svg></span><span class="at-label" style="font-size: 11.4px; line-height: 32px; height: 32px; color: rgb(255, 255, 255);">Facebook</span></a><a role="button" tabindex="0" class="at-icon-wrapper at-share-btn at-svc-twitter" style="background-color: rgb(29, 161, 242); border-radius: 0px;"><span class="at4-visually-hidden">Share to Twitter</span><span class="at-icon-wrapper" style="line-height: 32px; height: 32px; width: 32px;"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 32 32" version="1.1" role="img" aria-labelledby="at-svg-twitter-8" class="at-icon at-icon-twitter" style="fill: rgb(255, 255, 255); width: 32px; height: 32px;"><title id="at-svg-twitter-8">Twitter</title><g><path d="M27.996 10.116c-.81.36-1.68.602-2.592.71a4.526 4.526 0 0 0 1.984-2.496 9.037 9.037 0 0 1-2.866 1.095 4.513 4.513 0 0 0-7.69 4.116 12.81 12.81 0 0 1-9.3-4.715 4.49 4.49 0 0 0-.612 2.27 4.51 4.51 0 0 0 2.008 3.755 4.495 4.495 0 0 1-2.044-.564v.057a4.515 4.515 0 0 0 3.62 4.425 4.52 4.52 0 0 1-2.04.077 4.517 4.517 0 0 0 4.217 3.134 9.055 9.055 0 0 1-5.604 1.93A9.18 9.18 0 0 1 6 23.85a12.773 12.773 0 0 0 6.918 2.027c8.3 0 12.84-6.876 12.84-12.84 0-.195-.005-.39-.014-.583a9.172 9.172 0 0 0 2.252-2.336" fill-rule="evenodd"></path></g></svg></span><span class="at-label" style="font-size: 11.4px; line-height: 32px; height: 32px; color: rgb(255, 255, 255);">Twitter</span></a><a role="button" tabindex="0" class="at-icon-wrapper at-share-btn at-svc-pinterest_share" style="background-color: rgb(203, 32, 39); border-radius: 0px;"><span class="at4-visually-hidden">Share to Pinterest</span><span class="at-icon-wrapper" style="line-height: 32px; height: 32px; width: 32px;"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 32 32" version="1.1" role="img" aria-labelledby="at-svg-pinterest_share-9" class="at-icon at-icon-pinterest_share" style="fill: rgb(255, 255, 255); width: 32px; height: 32px;"><title id="at-svg-pinterest_share-9">Pinterest</title><g><path d="M7 13.252c0 1.81.772 4.45 2.895 5.045.074.014.178.04.252.04.49 0 .772-1.27.772-1.63 0-.428-1.174-1.34-1.174-3.123 0-3.705 3.028-6.33 6.947-6.33 3.37 0 5.863 1.782 5.863 5.058 0 2.446-1.054 7.035-4.468 7.035-1.232 0-2.286-.83-2.286-2.018 0-1.742 1.307-3.43 1.307-5.225 0-1.092-.67-1.977-1.916-1.977-1.692 0-2.732 1.77-2.732 3.165 0 .774.104 1.63.476 2.336-.683 2.736-2.08 6.814-2.08 9.633 0 .87.135 1.728.224 2.6l.134.137.207-.07c2.494-3.178 2.405-3.8 3.533-7.96.61 1.077 2.182 1.658 3.43 1.658 5.254 0 7.614-4.77 7.614-9.067C26 7.987 21.755 5 17.094 5 12.017 5 7 8.15 7 13.252z" fill-rule="evenodd"></path></g></svg></span><span class="at-label" style="font-size: 11.4px; line-height: 32px; height: 32px; color: rgb(255, 255, 255);">Pinterest</span><span class="at4-share-count-container" style="font-size: 11.4px; line-height: 32px; color: rgb(255, 255, 255);">11</span></a><a role="button" tabindex="0" class="at-icon-wrapper at-share-btn at-svc-odnoklassniki_ru" style="background-color: rgb(213, 120, 25); border-radius: 0px;"><span class="at4-visually-hidden">Share to Odnoklassniki</span><span class="at-icon-wrapper" style="line-height: 32px; height: 32px; width: 32px;"><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 32 32" version="1.1" role="img" aria-labelledby="at-svg-odnoklassniki_ru-10" class="at-icon at-icon-odnoklassniki_ru" style="fill: rgb(255, 255, 255); width: 32px; height: 32px;"><title id="at-svg-odnoklassniki_ru-10">Odnoklassniki</title><g><path d="M16.5 16.15A6.15 6.15 0 0 0 22.65 10c0-3.39-2.75-6.14-6.15-6.14-3.4 0-6.15 2.75-6.15 6.14.01 3.4 2.76 6.15 6.15 6.15zm0-9.17c1.67 0 3.02 1.35 3.02 3.02s-1.35 3.02-3.02 3.02-3.02-1.35-3.02-3.02 1.35-3.02 3.02-3.02zm7.08 9.92c-.35-.7-1.31-1.28-2.58-.27-1.73 1.36-4.5 1.36-4.5 1.36s-2.77 0-4.5-1.36c-1.28-1.01-2.24-.43-2.59.27-.6 1.22.08 1.8 1.62 2.79 1.32.85 3.13 1.16 4.3 1.28l-.98.98c-1.38 1.37-2.7 2.7-3.62 3.62-.55.55-.55 1.438 0 1.99l.17.17c.55.55 1.44.55 1.99 0l3.62-3.622 3.62 3.62c.55.55 1.44.55 1.99 0l.17-.17c.55-.55.55-1.44 0-1.99l-3.62-3.62-.98-.98c1.17-.12 2.96-.438 4.27-1.28 1.55-.988 2.23-1.58 1.62-2.788z"></path></g></svg></span><span class="at-label" style="font-size: 11.4px; line-height: 32px; height: 32px; color: rgb(255, 255, 255);">Odnoklassniki</span></a></div></div></div>
</div>
</div>
<!-- /uSocial -->
	



</div>

<div class="paginationstat">
	<div class="icleft"></div>


	<div class="icright"><a href="https://ravesli.com/urok-2-vvedenie-v-yazyki-programmirovaniya-c-i-s/" rel="next"><div class="text-paginationstat2">Урок №2. Введение в языки программирования C и С++<i class="fa fa-arrow-circle-right" aria-hidden="true"></i><span><i class="fa fa-arrow-circle-right fa-3x icon-pagination"></i></span></div></a></div>

</div>

<script>
$('.hidd').click(function() {
  $(this).toggleClass('active23').next()[$(this).next().is(':hidden') ? "slideDown" : "slideUp"](300);
});
</script>


	
<div class="relatedp">
		<script async="" src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle" style="display:block" data-ad-format="autorelaxed" data-ad-client="ca-pub-1157306330783763" data-ad-slot="2514287394"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>
	
</div>



<div class="comentu">

<div id="comments" class="comments-area">

			<h2 class="comments-title">
			 Комментариев: 55 		</h2>

		<ol class="comment-list">
				<li class="comment even thread-even depth-1 parent" id="comment-14493">
				<div id="div-comment-14493" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/3baf18eb6d5311f6d287e2193e32314a?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Andrew</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-14493">30 января 2021 в 10:29</a>		</div>

		<p>Добрый день, Юрий.<br>
Задам вопрос, который наверняка интересует многих.<br>
На сколько условных часов (дней, недель) рассчитан ваш курс при, допустим, пятидневной учебной неделе.<br>
 Понятно, что это очень условно и индивидуально, но я думаю такая статистика или что-то, типа "учебного плана", возможно у вас есть.<br>
 С уважением.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=14493#respond" data-commentid="14493" data-postid="1377" data-belowelement="div-comment-14493" data-respondelement="respond" data-replyto="Комментарий к записи Andrew" aria-label="Комментарий к записи Andrew">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor odd alt depth-2" id="comment-14516">
				<div id="div-comment-14516" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-14516">31 января 2021 в 23:10</a>		</div>

		<p>Здравствуйте! Как вы уже подметили, это очень условно и индивидуально, зависит от учащегося, его опыта и скорости прогрессирования, поэтому могу сказать только в общих чертах — без опыта за полгода-год можно пройти не спеша (1-2 урока в день). А то, как человек усваивает материал, сколько раз ему нужно перечитать то, что он не понял, делает ли он самостоятельно задания после уроков и проходит ли итоговые тесты — это всё также нужно учитывать.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=14516#respond" data-commentid="14516" data-postid="1377" data-belowelement="div-comment-14516" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment even thread-odd thread-alt depth-1 parent" id="comment-12302">
				<div id="div-comment-12302" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/d56eb4417f133ceb1979c942d19da5a3?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Ян</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-12302">7 сентября 2020 в 12:48</a>		</div>

		<p>Скажите пожалуйста, а будет-ли статья по написанию компилятора для своего языка программирования? Какие инструменты при этом нужно использовать? Какую литературу почитать? И т.д. А то до меня все никак не доходит как создаются языки программирования. Читал на других сайтах, но так ничего и не понял, ибо пишут поверхностно. Собственно хотелось-бы лучше узнать как это все взаимодействует между собой на практике…</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=12302#respond" data-commentid="12302" data-postid="1377" data-belowelement="div-comment-12302" data-respondelement="respond" data-replyto="Комментарий к записи Ян" aria-label="Комментарий к записи Ян">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment odd alt depth-2" id="comment-14310">
				<div id="div-comment-14310" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/32f9a6ecf4f230dcc5a7ecab75f1e206?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Даниил</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-14310">14 января 2021 в 12:19</a>		</div>

		<p>Эта тема довольно сложная. Наилучший вариант — найти "Книгу дракона" (она так и называется). Там подробно описано, как создаются языки, и как под них делаются компиляторы или интерпретаторы.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=14310#respond" data-commentid="14310" data-postid="1377" data-belowelement="div-comment-14310" data-respondelement="respond" data-replyto="Комментарий к записи Даниил" aria-label="Комментарий к записи Даниил">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment even thread-even depth-1" id="comment-12183">
				<div id="div-comment-12183" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/1ca2430ee8c5b971ea36ff6a5af54524?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Макс</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-12183">29 августа 2020 в 18:26</a>		</div>

		<p>Да, всё супер!  Ни разу не программист, но читается легко и интересно!<br>
🙂</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=12183#respond" data-commentid="12183" data-postid="1377" data-belowelement="div-comment-12183" data-respondelement="respond" data-replyto="Комментарий к записи Макс" aria-label="Комментарий к записи Макс">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment odd alt thread-odd thread-alt depth-1 parent" id="comment-12080">
				<div id="div-comment-12080" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/d56eb4417f133ceb1979c942d19da5a3?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Глеб</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-12080">24 августа 2020 в 22:15</a>		</div>

		<p>Как я рад что существует такой великолепный сайт, как Ravesli.com, где можно черпать глубокие знания по изучению С++. Это лучший сайт из всех которые я когда-либо находил. Единственное, есть только один небольшой минус, — это отсутствие других языков программирования. Хотелось-бы увидеть другие языки, к примеру — Java. Прошу курсы по Java добавить, т.к. нигде такой детально-изложенной информации по изучению не нашел…</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=12080#respond" data-commentid="12080" data-postid="1377" data-belowelement="div-comment-12080" data-respondelement="respond" data-replyto="Комментарий к записи Глеб" aria-label="Комментарий к записи Глеб">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor even depth-2" id="comment-12093">
				<div id="div-comment-12093" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-12093">25 августа 2020 в 17:38</a>		</div>

		<p>Пока что по Java ничего не планируется)</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=12093#respond" data-commentid="12093" data-postid="1377" data-belowelement="div-comment-12093" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment odd alt thread-even depth-1" id="comment-9609">
				<div id="div-comment-9609" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/d269584e9295118f80648048d8896168?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">cybersatori</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-9609">17 апреля 2020 в 16:31</a>		</div>

		<p>Поделюсь. На усвоение базового курса ушло 3 месяца и 330 часов (по 3 часа в день). Информация подана отлично и в базовых концепциях я теперь разбираюсь. Спасибо Юрию за перевод. Ничего более путного и сжатого в рунете нет по сабжу.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=9609#respond" data-commentid="9609" data-postid="1377" data-belowelement="div-comment-9609" data-respondelement="respond" data-replyto="Комментарий к записи cybersatori" aria-label="Комментарий к записи cybersatori">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment even thread-odd thread-alt depth-1" id="comment-9220">
				<div id="div-comment-9220" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/066d9187b32916bd606d9dadefe5c82a?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Сергей</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-9220">24 марта 2020 в 20:38</a>		</div>

		<p>наконец-то, я увидел свет. спасибо!</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=9220#respond" data-commentid="9220" data-postid="1377" data-belowelement="div-comment-9220" data-respondelement="respond" data-replyto="Комментарий к записи Сергей" aria-label="Комментарий к записи Сергей">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment odd alt thread-even depth-1 parent" id="comment-7410">
				<div id="div-comment-7410" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/432fcc01cab953cd26d2b9eecdfb7bf1?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Александр</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-7410">28 ноября 2019 в 04:36</a>		</div>

		<p>Здравствуйте Юрий! Прочитал все комментарии, благодарю вас за самоотверженность и желание учиться и учить. Уже больше года изучаю программирование на вашем сайте и понимаю что ещё не всё освоил и не во всём разобрался. Вы большой мостак в этом деле. Мне ещё работать и работать. И впрямь как будто не початый край. Снова с нуля. Творите У вас хорошо получается!</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=7410#respond" data-commentid="7410" data-postid="1377" data-belowelement="div-comment-7410" data-respondelement="respond" data-replyto="Комментарий к записи Александр" aria-label="Комментарий к записи Александр">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor even depth-2 parent" id="comment-7412">
				<div id="div-comment-7412" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-7412">28 ноября 2019 в 10:08</a>		</div>

		<p>Спасибо, мне очень приятно 😉</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=7412#respond" data-commentid="7412" data-postid="1377" data-belowelement="div-comment-7412" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment odd alt depth-3" id="comment-7800">
				<div id="div-comment-7800" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/4a18fba398800b748cd3dfe0a3bf5b69?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">xzxz</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-7800">21 декабря 2019 в 08:08</a>		</div>

		<p>да статья правда хорошая мне нравится все понятно</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=7800#respond" data-commentid="7800" data-postid="1377" data-belowelement="div-comment-7800" data-respondelement="respond" data-replyto="Комментарий к записи xzxz" aria-label="Комментарий к записи xzxz">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment even thread-odd thread-alt depth-1 parent" id="comment-4898">
				<div id="div-comment-4898" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/4ea980ec445ac0f601e06a31432b24dc?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Евгений</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-4898">19 мая 2019 в 10:51</a>		</div>

		<p>Сайт отличный. Помогает расширять свои знания в  IT</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=4898#respond" data-commentid="4898" data-postid="1377" data-belowelement="div-comment-4898" data-respondelement="respond" data-replyto="Комментарий к записи Евгений" aria-label="Комментарий к записи Евгений">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor odd alt depth-2" id="comment-5072">
				<div id="div-comment-5072" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-5072">6 июня 2019 в 15:07</a>		</div>

		<p>Очень надеюсь, что так и есть.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=5072#respond" data-commentid="5072" data-postid="1377" data-belowelement="div-comment-5072" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment even thread-even depth-1" id="comment-4724">
				<div id="div-comment-4724" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/870ae378343ae65c3617d805c84bd34f?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Вадим</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-4724">21 апреля 2019 в 23:19</a>		</div>

		<p>Привет! Очень интересная статья, благодарю за потраченое время и подробное разъяснение профанам.<br>
Особенно понравилось, упоминания Assembler. Было бы неплохо объяснить начинающим, что компьютер понимает только цифры, то что мы видим — является GUI, тоесть графической оболочкой. Самым лучшим примером, того как на самом деле должен выглядеть рабочий стол — является дистрибутив Arch.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=4724#respond" data-commentid="4724" data-postid="1377" data-belowelement="div-comment-4724" data-respondelement="respond" data-replyto="Комментарий к записи Вадим" aria-label="Комментарий к записи Вадим">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment odd alt thread-odd thread-alt depth-1" id="comment-4288">
				<div id="div-comment-4288" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/3ef9dc5fa91f4132849bd243afa4d67e?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Не до 4еловек</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-4288">5 марта 2019 в 11:55</a>		</div>

		<p>Спасибо огромное! Теперь буду учится)))))</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=4288#respond" data-commentid="4288" data-postid="1377" data-belowelement="div-comment-4288" data-respondelement="respond" data-replyto="Комментарий к записи Не до 4еловек" aria-label="Комментарий к записи Не до 4еловек">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment even thread-even depth-1" id="comment-4080">
				<div id="div-comment-4080" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/c83927980766a1ae38dc10ed99833544?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Creator Engines</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-4080">15 февраля 2019 в 18:43</a>		</div>

		<p>Здравствуйте Юра! Я хотел бы научиться написать 3D игровой движок какие уроки прочитать по этой теме? Спасибо за ответ заранее.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=4080#respond" data-commentid="4080" data-postid="1377" data-belowelement="div-comment-4080" data-respondelement="respond" data-replyto="Комментарий к записи Creator Engines" aria-label="Комментарий к записи Creator Engines">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment odd alt thread-odd thread-alt depth-1 parent" id="comment-3880">
				<div id="div-comment-3880" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/909590dab3712de7eedc84c3dc51a4b8?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Alexey</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-3880">24 января 2019 в 13:32</a>		</div>

		<p>Подскажите как вставлять код в комментарии, чтобы он сохранял структуру как в IDE(как примеры на сайте)? Использую Visual Studio.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=3880#respond" data-commentid="3880" data-postid="1377" data-belowelement="div-comment-3880" data-respondelement="respond" data-replyto="Комментарий к записи Alexey" aria-label="Комментарий к записи Alexey">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor even depth-2" id="comment-3882">
				<div id="div-comment-3882" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-3882">24 января 2019 в 13:57</a>		</div>

		<p>Форматирование кода задаётся специальным плагином — просто загружайте обычный код, а дальше я отформатирую его самостоятельно.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=3882#respond" data-commentid="3882" data-postid="1377" data-belowelement="div-comment-3882" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment odd alt thread-even depth-1 parent" id="comment-3734">
				<div id="div-comment-3734" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/48b82e5b2191f2232615319ab940c9d8?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Лиза</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-3734">5 января 2019 в 20:30</a>		</div>

		<p>Здраствуйте. Спасибо за такой понятный урок, но не совсем поняла, что значит таблица в конце. Спасибо.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=3734#respond" data-commentid="3734" data-postid="1377" data-belowelement="div-comment-3734" data-respondelement="respond" data-replyto="Комментарий к записи Лиза" aria-label="Комментарий к записи Лиза">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor even depth-2" id="comment-3735">
				<div id="div-comment-3735" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-3735">5 января 2019 в 20:40</a>		</div>

		<p>Привет. Это всего лишь начало — продолжайте обучение 🙂</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=3735#respond" data-commentid="3735" data-postid="1377" data-belowelement="div-comment-3735" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment odd alt thread-odd thread-alt depth-1 parent" id="comment-3141">
				<div id="div-comment-3141" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/806c32ef3e7555fc126ea4f1aca663fb?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">KanuTaH_KaKaxa</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-3141">23 сентября 2018 в 09:28</a>		</div>

		<p>Спасибо автору!!!<br>
Все предельно ясно разжовано.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=3141#respond" data-commentid="3141" data-postid="1377" data-belowelement="div-comment-3141" data-respondelement="respond" data-replyto="Комментарий к записи KanuTaH_KaKaxa" aria-label="Комментарий к записи KanuTaH_KaKaxa">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor even depth-2" id="comment-3142">
				<div id="div-comment-3142" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-3142">23 сентября 2018 в 11:59</a>		</div>

		<p>Спасибо, что читаешь 🙂</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=3142#respond" data-commentid="3142" data-postid="1377" data-belowelement="div-comment-3142" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment odd alt thread-even depth-1 parent" id="comment-3048">
				<div id="div-comment-3048" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/80566e54323f55fb06773b7d492f00e2?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Константин</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-3048">30 августа 2018 в 22:22</a>		</div>

		<p>Юра, значит мы вводим инструкции на высокоуровневом языке, компилятор переводит их в двоичный код, а процессор из этого двоичного кода еще какие-то инструкции ваяет? Просто из любопытства, если знаешь, напиши как они выглядят.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=3048#respond" data-commentid="3048" data-postid="1377" data-belowelement="div-comment-3048" data-respondelement="respond" data-replyto="Комментарий к записи Константин" aria-label="Комментарий к записи Константин">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment even depth-2" id="comment-3256">
				<div id="div-comment-3256" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/ed9b37e84688c0a414983103f83c9279?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Владимир</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-3256">24 октября 2018 в 18:41</a>		</div>

		<p>Микрокоманды для АЛУ, которое собсно и выполняет действия над битами данных.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=3256#respond" data-commentid="3256" data-postid="1377" data-belowelement="div-comment-3256" data-respondelement="respond" data-replyto="Комментарий к записи Владимир" aria-label="Комментарий к записи Владимир">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment odd alt thread-odd thread-alt depth-1 parent" id="comment-2746">
				<div id="div-comment-2746" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/5f0ea6bf897db4f2a1a05201a3c57b21?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Сергей</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-2746">10 июля 2018 в 08:30</a>		</div>

		<p>Подскажите пожалуйста стоит мне начинать учить с c++ или лучше начать попроще изучить язык для понимания, до этого не занимался программированием. Спасибо!</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=2746#respond" data-commentid="2746" data-postid="1377" data-belowelement="div-comment-2746" data-respondelement="respond" data-replyto="Комментарий к записи Сергей" aria-label="Комментарий к записи Сергей">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor even depth-2" id="comment-2762">
				<div id="div-comment-2762" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-2762">12 июля 2018 в 21:22</a>		</div>

		<p>Попробуйте и то, и другое. Затем и определите, что вам лучше подходит.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=2762#respond" data-commentid="2762" data-postid="1377" data-belowelement="div-comment-2762" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment odd alt thread-even depth-1 parent" id="comment-2699">
				<div id="div-comment-2699" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/5bdce745c6e211f44c2276c313268217?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">oleg</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-2699">30 июня 2018 в 09:12</a>		</div>

		<p>Помогите — не понял.<br>
Машинный код 10110000 01100001 получается в результате инструкции a = 97;</p>
<p>10110000 == 176<br>
01100001 == 97<br>
'a' == 97<br>
'=' == 61<br>
'пробел' == 32<br>
';' == 59</p>
<p>Как формируется машинный код ?<br>
Спасибо.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=2699#respond" data-commentid="2699" data-postid="1377" data-belowelement="div-comment-2699" data-respondelement="respond" data-replyto="Комментарий к записи oleg" aria-label="Комментарий к записи oleg">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment even depth-2" id="comment-3255">
				<div id="div-comment-3255" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/80566e54323f55fb06773b7d492f00e2?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Константин</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-3255">24 октября 2018 в 18:22</a>		</div>

		<p>Олег, а ты выдели свой вопрос и спроси у Гугла — прозреешь!</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=3255#respond" data-commentid="3255" data-postid="1377" data-belowelement="div-comment-3255" data-respondelement="respond" data-replyto="Комментарий к записи Константин" aria-label="Комментарий к записи Константин">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment odd alt thread-odd thread-alt depth-1" id="comment-2592">
				<div id="div-comment-2592" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/1fff60cd93bd071a5210c2dd629fa689?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Blackson</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-2592">8 июня 2018 в 22:05</a>		</div>

		<p>Отличный урок !</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=2592#respond" data-commentid="2592" data-postid="1377" data-belowelement="div-comment-2592" data-respondelement="respond" data-replyto="Комментарий к записи Blackson" aria-label="Комментарий к записи Blackson">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment even thread-even depth-1 parent" id="comment-2543">
				<div id="div-comment-2543" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/7a55ce2b761fab80011d568f0d9e9732?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Марина</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-2543">2 июня 2018 в 11:08</a>		</div>

		<p>Кажется, на просторах интернета я откопала сокровище) Такое понятное изложение информации на вес золота.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=2543#respond" data-commentid="2543" data-postid="1377" data-belowelement="div-comment-2543" data-respondelement="respond" data-replyto="Комментарий к записи Марина" aria-label="Комментарий к записи Марина">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor odd alt depth-2" id="comment-2545">
				<div id="div-comment-2545" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-2545">2 июня 2018 в 11:17</a>		</div>

		<p>Спасибо 🙂</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=2545#respond" data-commentid="2545" data-postid="1377" data-belowelement="div-comment-2545" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment even thread-odd thread-alt depth-1 parent" id="comment-1891">
				<div id="div-comment-1891" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/14a6e20732e12c262860e04f2f5ed987?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Семён</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1891">12 февраля 2018 в 22:11</a>		</div>

		<p>Просто великолепно ! Я скажу очень бонально : я тоже искал , что-то подобное , находил , но обучение там шло очень не поэтапно . Например , тоже же самый St***k ( не буду рекламировать ) , который на одном уроке давал действительные числа и в тоже время  множество функций , таже самая break …..<br>
Но вот я нашел вас …. Сам тоже изучаю английский язык и совмещать полезно .  У вас очень хорошая манера излагаться  и главное : поэтапная подача . Пусть даже первая часть ( глава ) , которой даже опытные IT -специалисты  крайне мало уделяют внимание .  Ещё бы слепому набор научится<br>
Сам люблю технологии , новинки и т.д  , но вот только в 16-17 лет дошли руки до обучения программ.Но в тоже самое время считаю , что возраст 16-20 лет  как раз для этого подходит , но учится не когда не поздно .<br>
Огромное спасибо , добавился б в друзья , но вы не горите какой у вас name user в ВК . </p>
<p>Ещё раз огромное спасибо … Путь начался ⚡⚡⚡⭐⭐</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1891#respond" data-commentid="1891" data-postid="1377" data-belowelement="div-comment-1891" data-respondelement="respond" data-replyto="Комментарий к записи Семён" aria-label="Комментарий к записи Семён">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor odd alt depth-2 parent" id="comment-1899">
				<div id="div-comment-1899" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1899">13 февраля 2018 в 17:52</a>		</div>

		<p>Я в свои 17-18 лет тоже, когда нужно было уже что-то учить по C++ (в колледже этот язык программирования был основным) — пытался искать на просторах Рунета годные уроки. Нашел несколько сайтов, и как вы тоже говорите, сегодня учим "Hello, World!", завтра ООП, послезавтра паттерны проектирования и всё в этом роде. Так и задумался, что нет одного сайта в Рунете по изучению C++, где всё было бы поэтапно, с самых мелочей и уже до базовых вещей.</p>
<p>Насчет учиться — учиться никогда не поздно, но чем раньше, тем лучше 🙂</p>
<p>Спасибо, что читаете.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1899#respond" data-commentid="1899" data-postid="1377" data-belowelement="div-comment-1899" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment even depth-3 parent" id="comment-1904">
				<div id="div-comment-1904" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/14a6e20732e12c262860e04f2f5ed987?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Семён</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1904">13 февраля 2018 в 23:00</a>		</div>

		<p>Успехов и удачи во всём !</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1904#respond" data-commentid="1904" data-postid="1377" data-belowelement="div-comment-1904" data-respondelement="respond" data-replyto="Комментарий к записи Семён" aria-label="Комментарий к записи Семён">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor odd alt depth-4" id="comment-1905">
				<div id="div-comment-1905" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1905">14 февраля 2018 в 10:27</a>		</div>

		<p>Спасибо 🙂</p>

		
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment even depth-3" id="comment-4388">
				<div id="div-comment-4388" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/e8bebd14b05dddf8481aa3cd78e1069f?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Waldemar</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-4388">15 марта 2019 в 22:04</a>		</div>

		<p>Спасибо тебе, человечище! Хочу попробовать себя фрилансером после этого курса.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=4388#respond" data-commentid="4388" data-postid="1377" data-belowelement="div-comment-4388" data-respondelement="respond" data-replyto="Комментарий к записи Waldemar" aria-label="Комментарий к записи Waldemar">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment odd alt thread-even depth-1 parent" id="comment-1762">
				<div id="div-comment-1762" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/9c6c9c8a2cd3afca545d65fafcd2a79e?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">ali</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1762">24 января 2018 в 21:15</a>		</div>

		<p>Привет, а практика будет? Тесты, задания и всё такое.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1762#respond" data-commentid="1762" data-postid="1377" data-belowelement="div-comment-1762" data-respondelement="respond" data-replyto="Комментарий к записи ali" aria-label="Комментарий к записи ali">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor even depth-2" id="comment-1763">
				<div id="div-comment-1763" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1763">24 января 2018 в 22:07</a>		</div>

		<p>Всё есть в следующих уроках.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1763#respond" data-commentid="1763" data-postid="1377" data-belowelement="div-comment-1763" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment odd alt thread-odd thread-alt depth-1" id="comment-1756">
				<div id="div-comment-1756" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/9c6c9c8a2cd3afca545d65fafcd2a79e?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">ali</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1756">23 января 2018 в 09:46</a>		</div>

		<p>Хорошо, спасибо</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1756#respond" data-commentid="1756" data-postid="1377" data-belowelement="div-comment-1756" data-respondelement="respond" data-replyto="Комментарий к записи ali" aria-label="Комментарий к записи ali">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment even thread-even depth-1 parent" id="comment-1646">
				<div id="div-comment-1646" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/cd5c7619e13819c8a3c7ba03c5b7f1bc?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Борис</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1646">6 января 2018 в 02:19</a>		</div>

		<p>Здравствуйте. Приятно удивлён способом изложения материала. Начало курса очень хорошее. Неделю искал по этой теме и склонился к мысли, что люди либо не умеют изложить суть понятно, либо у них совсем другие цели.<br>
   Большой плюс, что вы рассматриваете решение задачи при помощи разных программ.<br>
    Так же заслуживает внимания мысль одновременного изучения английского со слепым методом печатания. Всё к одному.<br>
   Что там получится у меня, не важно, мне на работу уже не надо, но ради интереса попробую.<br>
   Успехов в достойной профессии. Спасибо.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1646#respond" data-commentid="1646" data-postid="1377" data-belowelement="div-comment-1646" data-respondelement="respond" data-replyto="Комментарий к записи Борис" aria-label="Комментарий к записи Борис">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor odd alt depth-2 parent" id="comment-1654">
				<div id="div-comment-1654" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1654">8 января 2018 в 20:22</a>		</div>

		<p>Здравствуйте. Приятно, что моя работа приносит кому-то пользу. Программирование и английский идут друг с другом (это не значит, что первое не может быть без второго) и, как по мне, отличный способ изучая программирование, подтягивать английский. Слепой набор очень экономит время при работе с компьютером вообще. Надеюсь, ваше желание не угаснет изучать программирование и дальше. Если есть к этому желание, то это довольно-таки интересное занятие.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1654#respond" data-commentid="1654" data-postid="1377" data-belowelement="div-comment-1654" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment even depth-3 parent" id="comment-1745">
				<div id="div-comment-1745" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/9c6c9c8a2cd3afca545d65fafcd2a79e?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">ali</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1745">22 января 2018 в 09:57</a>		</div>

		<p>Здравствуйте. Мне 16 и дело в том что я вообще не много знаю о компьютерах, о языках и обо всем этом можно сказать даже ничего не знаю. Я начал учить английский и хочу научиться языкам программирования подскажите что делать я с правильного сайта начал?</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1745#respond" data-commentid="1745" data-postid="1377" data-belowelement="div-comment-1745" data-respondelement="respond" data-replyto="Комментарий к записи ali" aria-label="Комментарий к записи ali">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor odd alt depth-4" id="comment-1748">
				<div id="div-comment-1748" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1748">22 января 2018 в 13:55</a>		</div>

		<p>Привет, попробуй. Увидишь, есть ли польза или нет.</p>

		
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment even thread-odd thread-alt depth-1 parent" id="comment-1545">
				<div id="div-comment-1545" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/70e5a9e9c07ea46c3e55540b76e676d7?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Ильнур</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1545">9 декабря 2017 в 21:58</a>		</div>

		<p>Учитель!!!! А задачки будут?<br>
Спасибо тебе за труд!!!</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1545#respond" data-commentid="1545" data-postid="1377" data-belowelement="div-comment-1545" data-respondelement="respond" data-replyto="Комментарий к записи Ильнур" aria-label="Комментарий к записи Ильнур">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor odd alt depth-2" id="comment-1546">
				<div id="div-comment-1546" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1546">9 декабря 2017 в 23:11</a>		</div>

		<p>Да, вот <strong><a href="https://ravesli.com/praktika-chast-1/" rel="noopener noreferrer" target="_blank">первая часть задачек по C++</a></strong>, дальше больше)</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1546#respond" data-commentid="1546" data-postid="1377" data-belowelement="div-comment-1546" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment even thread-even depth-1 parent" id="comment-1531">
				<div id="div-comment-1531" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/5f0ea6bf897db4f2a1a05201a3c57b21?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Сергей</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1531">4 декабря 2017 в 18:54</a>		</div>

		<p>Добрый вечер! Я читаю ваши уроки и меня увлекает и нравится, хочу научиться программировать, сначаля для общего развития, а потом как пойдёт, вдруг по этой сфере пойду вперёд. Я хочу спросить у вас, сам результат той программы или игры, как мне его видеть в конечном результате. Я имею в виду, например пишу игру какую-нибудь, написал алгоритмы и для себя видеть результат, области карты которой написал, цвет, фон, герой которого написал и т.д. Подскажите пожалуйста, спасибо!</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1531#respond" data-commentid="1531" data-postid="1377" data-belowelement="div-comment-1531" data-respondelement="respond" data-replyto="Комментарий к записи Сергей" aria-label="Комментарий к записи Сергей">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor odd alt depth-2" id="comment-1533">
				<div id="div-comment-1533" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1533">5 декабря 2017 в 12:59</a>		</div>

		<p>Привет. Вам её нужно скомпилировать и запустить. Смотрите ‘<a href="https://ravesli.com/urok-5-kompilyatsiya-vashej-pervoj-programmy/" rel="noopener noreferrer" target="_blank"><strong>Урок 5. Компиляция вашей первой программы</strong></a>‘.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1533#respond" data-commentid="1533" data-postid="1377" data-belowelement="div-comment-1533" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment even thread-odd thread-alt depth-1" id="comment-1491">
				<div id="div-comment-1491" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/22a0c577225c6c5bcd44ba6fc0ac0531?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Irina</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1491">24 ноября 2017 в 15:55</a>		</div>

		<p>Наконец-то снова появилось желание учится по программиста. Третий год учусь уже на эту специальности и руки совсем начали опускаться. Потому что всё я слышу эти 3 года — мышка с шариком, монитор монохромный, таблицы в эксель.<br>
И тут этот сайт просто как глоток свежего воздуха!</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1491#respond" data-commentid="1491" data-postid="1377" data-belowelement="div-comment-1491" data-respondelement="respond" data-replyto="Комментарий к записи Irina" aria-label="Комментарий к записи Irina">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment odd alt thread-even depth-1" id="comment-1448">
				<div id="div-comment-1448" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/3a652a676fa711e8683c394c98a965a8?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Ибрагим</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-1448">14 ноября 2017 в 18:18</a>		</div>

		<p>Спасибо большое брат, 2 месяца искал что-то похожее на это, век не забуду!</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=1448#respond" data-commentid="1448" data-postid="1377" data-belowelement="div-comment-1448" data-respondelement="respond" data-replyto="Комментарий к записи Ибрагим" aria-label="Комментарий к записи Ибрагим">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment even thread-odd thread-alt depth-1 parent" id="comment-887">
				<div id="div-comment-887" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/978a8be7fd6105e893c4cdb772e021ff?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Ivanshka</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-887">7 июля 2017 в 20:47</a>		</div>

		<p>Мне всего 16, неплохо знаю PascalABC.NET (пробовал написать небольшую игру, кое-что вышло, но до ума не довел из-за тормозов то ли языка, то ли железа, то ли кривости моих рук), HTML 5 и CSS 3 (пробовал сайт писать из интереса). В общем, кодить — моё хобби. Есть мечта (написать игру с какой-нибудь командой) и желание учиться, чтобы писать годные вещи, а не кучу говнокода, а ты пишешь такие уроки! Большое спасибо тебе, Юра!)</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=887#respond" data-commentid="887" data-postid="1377" data-belowelement="div-comment-887" data-respondelement="respond" data-replyto="Комментарий к записи Ivanshka" aria-label="Комментарий к записи Ivanshka">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor odd alt depth-2" id="comment-888">
				<div id="div-comment-888" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-888">7 июля 2017 в 22:30</a>		</div>

		<p>16 лет — как раз золотое время для изучения программирования. Больше практики, своих проектов и всё обязательно получиться!)</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=888#respond" data-commentid="888" data-postid="1377" data-belowelement="div-comment-888" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		<li class="comment even thread-even depth-1" id="comment-817">
				<div id="div-comment-817" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/261ab6305cb28869bf911db26f8aa573?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">DEADLIGHT</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-817">22 июня 2017 в 21:31</a>		</div>

		<p>спасибо за ресурс. начну свое самообучение…</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=817#respond" data-commentid="817" data-postid="1377" data-belowelement="div-comment-817" data-respondelement="respond" data-replyto="Комментарий к записи DEADLIGHT" aria-label="Комментарий к записи DEADLIGHT">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
		<li class="comment odd alt thread-odd thread-alt depth-1 parent" id="comment-797">
				<div id="div-comment-797" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://secure.gravatar.com/avatar/b4e1557f2c961fb2239a4bd8532b2cd4?s=50&amp;d=monsterid&amp;r=g" width="50" height="50" alt="Аватар" class="avatar avatar-50wp-user-avatar wp-user-avatar-50 alignnone photo avatar-default ">			<cite class="fn">Дмитрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-797">19 июня 2017 в 11:09</a>		</div>

		<p>Спасибо!<br>
Благодаря тебе у меня вернулось желание обучаться на программиста.<br>
Поступаю на второй курс, надеюсь, не слишком поздно начал)</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=797#respond" data-commentid="797" data-postid="1377" data-belowelement="div-comment-797" data-respondelement="respond" data-replyto="Комментарий к записи Дмитрий" aria-label="Комментарий к записи Дмитрий">Ответить</a></div>
				</div>
				<ol class="children">
		<li class="comment byuser comment-author-yura_ravesli bypostauthor even depth-2" id="comment-799">
				<div id="div-comment-799" class="comment-body">
				<div class="comment-author vcard">
			<img src="https://ravesli.com/wp-content/uploads/2019/03/vkpablik3-150x150.jpg" width="50" height="50" alt="Юрий" class="avatar avatar-50 wp-user-avatar wp-user-avatar-50 alignnone photo">			<cite class="fn">Юрий</cite><span class="says">:</span>		</div>
		
		<div class="comment-meta commentmetadata">
			<a href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/#comment-799">19 июня 2017 в 15:21</a>		</div>

		<p>Поверь, никогда не поздно, лишь бы нравилось.</p>

		<div class="reply"><a rel="nofollow" class="comment-reply-link" href="https://ravesli.com/urok-1-vvedenie-v-programmirovanie/?replytocom=799#respond" data-commentid="799" data-postid="1377" data-belowelement="div-comment-799" data-respondelement="respond" data-replyto="Комментарий к записи Юрий" aria-label="Комментарий к записи Юрий">Ответить</a></div>
				</div>
				</li><!-- #comment-## -->
</ol><!-- .children -->
</li><!-- #comment-## -->
		</ol><!-- .comment-list -->

		
		
		<div id="respond" class="comment-respond">
		<h3 id="reply-title" class="comment-reply-title">Добавить комментарий <small><a rel="nofollow" id="cancel-comment-reply-link" href="/urok-1-vvedenie-v-programmirovanie/#respond" style="display:none;">Отменить ответ</a></small></h3><form action="https://ravesli.com/wp-comments-post.php" method="post" id="commentform" class="comment-form"><p class="comment-notes">Ваш E-mail не будет опубликован. Обязательные поля помечены <span class="required">*</span></p><p class="comment-form-author"><label for="author">Имя <span class="required">*</span></label> <input id="author" name="author" type="text" value="" size="30" maxlength="245" required="required"></p>
<p class="comment-form-email"><label for="email">Email <span class="required">*</span></label> <input id="email" name="email" type="text" value="" size="30" maxlength="100" required="required"></p>

<p class="comment-form-comment"><label for="comment">Комментарий</label> <textarea id="comment" name="comment" cols="45" rows="8" maxlength="65525" required="required"></textarea></p><p class="comment-form-cookies-consent" style="clear:both;"><input id="wp-comment-cookies-consent" name="wp-comment-cookies-consent" type="checkbox" value="yes"><label for="wp-comment-cookies-consent">Сохранить моё Имя и E-mail. Видеть комментарии, отправленные на модерацию</label></p>
<p class="comment-form-subscriptions"><label for="subscribe-reloaded"><input type="checkbox" name="subscribe-reloaded" id="subscribe-reloaded" value="yes"> Получать уведомления о новых комментариях по электронной почте. Вы можете <a href="https://ravesli.com/comment-subscriptions/?srp=1377&amp;srk=435d14f705f54cb7e326304fc1c8089c&amp;sra=s&amp;srsrc=f">подписаться</a> без комментирования.</label></p><p class="form-submit"><input name="submit" type="submit" id="submit" class="submit" value="Отправить комментарий"> <input type="hidden" name="comment_post_ID" value="1377" id="comment_post_ID">
<input type="hidden" name="comment_parent" id="comment_parent" value="0">
</p><p style="display: none;"><input type="hidden" id="akismet_comment_nonce" name="akismet_comment_nonce" value="1f05578aeb"></p><textarea name="ak_hp_textarea" cols="45" rows="8" maxlength="100" style="display: none !important;"></textarea><input type="hidden" id="ak_js" name="ak_js" value="1620930140450"></form>	</div><!-- #respond -->
	

</div><!-- #comments --></div>


</div>
