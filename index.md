---
layout: home
---
<p class="alert"><b>Please note:</b> If Donald Trump is indicted between June 7 and June 15 2023, this site will not be updated because I am at literal actual Disney World with my family. <i>Sorry, not sorry.</i></p>

<p class="intro"><b>Previously:</b> {{ site.data.news.news[0].yesterday }}</p>
<h2 class="today"><time class="timeago" datetime="{{ site.data.news.news[0].date }}">{{ site.data.news.news[0].date }}</time>, {{ site.data.news.news[0].date | date: "%A, %B %e, %Y" }}</h2>
<ul class="today">
{% for today in site.data.news.news[0].todays %}
 <li>{{ today.item }} <span class="small">{% if today.source != null %}(Source: <a href="{{ today.url }}">{{ today.source }}</a>){% endif %}</span></li>
{% endfor %}
  </ul>

<p class="outtro"><b>What's coming next:</b> {{ site.data.news.news[0].tomorrow }}</p>


<!-- pre-indictment state DO NOT FORGET TO ADJUST THE FOOTER AND THE LAYOUT ONCE THINGS GO LIVE LIVE 
Hi there,

So Donald Trump has been indicted! A lot of things are going to happen now and this site and the corresponding newsletter will update regularly with news, so you don't have to track the ins-and-outs of all of this. Instead, I will. _Shudders_.

Yes, I'm literally writing the first edition right now. _Oh no_.

Hi, I'm <a href="https://dansinker.com">Dan Sinker</a> and during the two Trump impeachment proceedings, I wrote the <a href="https://impeachment.fyi">impeachment.fyi</a> newsletter and for some reason I've forgotten how much work that was and am doing it again. Sign up to get these updates delivered to you, because I guess we're really doing this:
-->
