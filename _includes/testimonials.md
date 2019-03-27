<img class="head" src="/assets/testimonials.png">

{% assign testimonials = site.testimonials | reverse %}
{% for testimonial in testimonials %}
  <div class="testimonial">
      <blockquote>{{ testimonial.content | markdownify }}</blockquote>
      <cite>
        <span class="name">{{ testimonial.name }}</span> 
        <span class="title">{{testimonial.title}}</span>
      </cite>
   </div>
{% endfor %}