<script>
	import {Container, Grid, SvelteUIProvider} from '@svelteuidev/core'
</script>

<SvelteUIProvider themeObserver="dark">
      <Container>
         <div class="app">
            <header>
               <Grid>
                  <Grid.Col span={4}>
                     <h1>Furniture factory management</h1>
                  </Grid.Col>
                  <Grid.Col span={8}>
                     <nav class="menu">
                        <ul>
                           <li><a href="/">List of orders</a></li>
                           <li><a href="/order">Make order</a></li>
                           <li><a href="/production">Production</a></li>
                        </ul>
                     </nav>
                  </Grid.Col>
               </Grid>
            </header>
            <slot></slot>
         </div>
      </Container>
</SvelteUIProvider>

<style>
   .app {
      background: #fff;
      padding: 2rem;
      margin: 2rem 0;
      border-radius: 1rem;
   }
   .menu ul {
      list-style: none;
      display: flex;
      gap: 1.5rem;
      justify-content: center;
   }
</style>