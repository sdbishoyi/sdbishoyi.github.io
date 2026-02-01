I can write instructions about managing the website here. As of 7/27/2024, I have forgotten what files need to be changed.

*********************** On 7/27/2024
    |=============|
The | _config.yml | file
    |=============|
    
If there is something here thatyou don't understand, you can give this file to ChatGPT to explain it to you.

************************************** In _data/navigation.yml ************************************************

I can see the links that appear on the website.

******************************************* The _pages folder ***************************************************

In this folder, the files that contain important text are about.md, blog.md, cv.md, projects.md, publications.md, research.md
                       |=======| 
markdown.md located in |_pages/| is important.
                       |=======| 
******************************************** The _posts folder *************************************************

contains samples of blog posts. Visit https://academicpages.github.io/ to checkout the model webpage.

Also checkout https://jayrobwilliams.com/posts/2020/06/academic-website/

**********************  On 04/11/2025

A standard format for a commit message in this repo could be "what changed in which file". This format can be changed in the future if necessary.

proposed change : 1. The font appearing at the top of the page in the horizontal bar has to be made bigger. It goes as Som Dev Bishoyi ... Research ... Publications etc

2. Include "Teaching" section in the header --> done by changing the navigation.yml file inside _data


****************************************** On 04/21/2025

1. There is a piece of code that must be included in files ending with either .md or .html in the _pages directory. This piece
sort of iterates over content in folders like _publications and _teaching or _posts to extract the content written in separate
markdown files in this folders.

This code looks like 

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.posts %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
    <h2 id="{{ year | slugify }}" class="archive__subtitle">{{ year }}</h2>
    {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}

2. We are ready to write blogs and add papers as they come. Next TODOS are to add in research details, teaching details and a blog. Also organize the config.yml file
by looking at the website's corresponding file.

3. How would you add pictures to convey your research. Also place a picture in the background.