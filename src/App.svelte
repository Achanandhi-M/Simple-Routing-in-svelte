<script>

  import {Router ,Route,Link} from "svelte-routing";
  import Home from "./home.svelte"
  import About from "./about.svelte";
    import Projects from "./Projects.svelte";
</script>
<Router>
  <nav>
   <Link to="/">Home</Link>
    <Link to="about">About</Link>
    <Link to="projects">projects</Link>
  </nav>
  <div>
   <Route path="/" component ="{Home}" />
    <Route path="about" component="{About}" />
    <Route path="projects" component="{Projects}" />
  </div>
</Router>
