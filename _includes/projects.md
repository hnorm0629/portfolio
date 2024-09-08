<h2 id="projects" style="margin: 2px 0px -15px;">Projects</h2>

<div class="projects">
<ol class="bibliography">

{% for link in site.data.projects.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% if link.course %} 
    <abbr class="badge">{{ link.course }}</abbr>
    {% endif %}
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="author">{{ link.description }}</div>
      <div class="periodical"><em>{{ link.date }}</em>
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>



<!-- ## Projects

### Realistic Ray-Traced Scene Using Blender's Cycles Engine

1. **[Publication Title 1](link_to_pdf)**  
   _Author 1, Author 2, Author 3_  
   *date Name or Journal*  
   [PDF](link_to_pdf) | [Code](link_to_code) | [Project Page](link_to_project_page) | [BibTex](link_to_bibtex)  
   _Note: Special note or additional information_  -->


<!-- The final project for CS148 (Intro Computer Graphics) was to create a visually compelling image using Blender's Cycles ray-tracing engine, showcasing your skills in geometry, materials, and textures. The project required me to model the primary geometry from scratch, apply custom UV mapping and texturing, and leverage the advantages of ray-tracing such as realistic lighting, shadows, and reflections. Additionally, I had to incorporate at least one advanced feature in Blender, like depth of field or volumetrics, to enhance the artistic quality of my scene.

I decided to recreate a scene from the videogame _Stray_, where you play as a cat exploring a dilapidated, underground city populated with robots. Every piece of geometry in my scene was created from scratch, except for the cat. This includes the neon sign, which is the main geometry/focus of my scene. I modeled the sign off an official image of the game asset, but I didn’t reference any tutorials to do so. I will include the reference photo and final image below. -->
