<script>
    import { goto } from '$app/navigation';
  </script>
  
  <nav>
    <ul>
      <li><a href="/" on:click|preventDefault={() => goto('/')}>Home</a></li>
      <li><a href="/hikes" on:click|preventDefault={() => goto('/hikes')}>Hikes</a></li>
      <li><a href="/about" on:click|preventDefault={() => goto('/about')}>About</a></li>
      <li><a href="/contact" on:click|preventDefault={() => goto('/contact')}>Contact</a></li>
    </ul>
  </nav>
  
  <style>
    nav {
      background-color: #333;
      overflow: hidden;
    }
  
    nav ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
    }
  
    nav ul li {
      float: left;
    }
  
    nav ul li a {
      display: block;
      color: white;
      text-align: center;
      padding: 14px 16px;
      text-decoration: none;
    }
  
    nav ul li a:hover {
      background-color: #111;
    }
  </style>