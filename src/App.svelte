<script lang="ts">
  import { fade } from 'svelte/transition';

  let events: any[] = [];  // Define the type for events if you know its structure
  const handleEventDrop = (event: any) => {  // Define event type if possible
    console.log("Event dropped:", event);
  };
</script>


<div class="min-h-screen bg-[#f8f8f6]">
<!-- Header -->


<header class="border-b">
  <div class="container mx-auto px-4 py-4 flex justify-between items-center">
    <div class="flex items-center flex-column">
      <svg class="h-6 w-6">
        <img src="./logo.jpg" alt="Logo" height="250" width="220">
      </svg>
      <span class="font-bold text-xl">CardSched</span>
    </div>
    <nav>
      <a href="/docs" class="btn ghost">Documentation</a>
    </nav>
  </div>
</header>

<!-- Hero Section -->
<section class="py-20 px-4" in:fade>
  <div class="container mx-auto max-w-4xl text-center">
    <svg class="h-20 w-20 mx-auto mb-8">
      <!-- Add appropriate Calendar SVG content here -->
    </svg>
    <h1 class="text-4xl md:text-6xl font-bold mb-6">
      Beautiful Card-Based Scheduling
    </h1>
    <p class="text-xl text-gray-600 mb-8 max-w-2xl mx-auto">
      CardSched is a simple React component library for building intuitive and beautiful card-based scheduling interfaces.
    </p>
    <div class="flex gap-4 justify-center">
      <a href="/docs" class="btn lg">Get Started</a>
      <a href="https://github.com/DavidNzube101/cardsched" class="btn lg outline">GitHub</a>
    </div>
  </div>
</section>

<!-- Features -->
<section class="py-20 bg-gray-50" in:fade>
  <div class="container mx-auto px-4">
    <h2 class="text-3xl font-bold text-center mb-12">Key Features</h2>
    <div class="grid md:grid-cols-3 gap-8 max-w-5xl mx-auto">
      <div class="p-6 bg-white rounded-lg shadow-sm">
        <h3 class="font-semibold text-xl mb-3">Intuitive Interface</h3>
        <p class="text-gray-600">
          Drag-and-drop scheduling with smooth animations and responsive design.
        </p>
      </div>
      <div class="p-6 bg-white rounded-lg shadow-sm">
        <h3 class="font-semibold text-xl mb-3">Customizable</h3>
        <p class="text-gray-600">
          Fully customizable themes and components to match your brand.
        </p>
      </div>
      <div class="p-6 bg-white rounded-lg shadow-sm">
        <h3 class="font-semibold text-xl mb-3">Developer Friendly</h3>
        <p class="text-gray-600">
          TypeScript support, comprehensive documentation, and easy integration.
        </p>
      </div>
    </div>
  </div>
</section>

<!-- Example Section -->
<section class="py-20" in:fade>
  <div class="container mx-auto px-4">
    <h2 class="text-3xl font-bold text-center mb-12">Simple to Use</h2>
    <div class="max-w-3xl mx-auto bg-gray-900 rounded-lg p-6">
      <pre class="text-gray-100 overflow-x-auto">
        <code>
{`<script>
import { CardSched } from 'cardsched';

let events = [];
const handleEventDrop = (event: any) => {
  console.log("Event dropped:", event);
};
</script>

<CardSched
events={events}
onEventDrop={handleEventDrop}
theme="light"
/>`}
        </code>
      </pre>
    </div>
  </div>
</section>

<!-- Footer -->
<footer class="border-t py-12">
  <div class="container mx-auto px-4 text-center text-gray-600">
    <p>© {new Date().getFullYear()} CardSched. All rights reserved. By <a href="https://www.github.com/DavidNzube101">David Nzube</a></p>
  </div>
</footer>
</div>
