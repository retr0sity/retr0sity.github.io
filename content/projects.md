---
title: "Projects"
---
{{< rawhtml >}}
<div id="projects-container" style="width: 100%; min-height: 2000px;">
  <iframe src="/github-projects.html" 
          id="projects-iframe"
          width="100%" 
          height="2000px" 
          style="border: none; display: block;">
  </iframe>
</div>

<script>
  window.addEventListener('message', function(event) {
    if (event.data && event.data.height) {
      document.getElementById('projects-iframe').style.height = event.data.height + 'px';
    }
  }, false);
  
  // Fallback: set large height after load
  setTimeout(function() {
    document.getElementById('projects-iframe').style.height = '2000px';
  }, 2000);
</script>
{{< /rawhtml >}}