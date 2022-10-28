<script lang="ts">
    import rt1 from "./rt1.svelte";
    import FourOhFour from "./FourOhFour.svelte";
    import { Router } from "svelte-router-spa";
    import Slash from "./Slash.svelte";
    import LogoBarHeader from "./infra/LogoBarHeader.svelte";
    import NavBar from "./infra/NavBar.svelte";

    const routes = [
        {
            name: "/",
            component: Slash
        },
      {
        name: "namee",
        component: rt1,
      },
      {
        name: "404",
        component: FourOhFour
      }
    ]


</script>

<LogoBarHeader/>
<NavBar/>

<Router {routes}/>