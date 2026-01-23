+++
title = "Sidebar"
weight = 120
description = "Fixed sidebar layout with collapsible sections using details/summary semantic tags."
+++

Use `.sidebar` on an `<aside>` and `<main>` for the main content area. Navigation must use semantic `<nav><ul><li>` structure.

<div class="sidebar-example">
{% demo() %}
```html
<aside class="sidebar">
  <h4>Dashboard</h4>
  <nav>
    <ul>
      <li><a href="#" aria-current="page">Home</a></li>
      <li><a href="#">Users</a></li>
      <li>
        <details open>
          <summary>Settings</summary>
          <ul>
            <li><a href="#">General</a></li>
            <li><a href="#">Security</a></li>
            <li><a href="#">Billing</a></li>
          </ul>
        </details>
      </li>
    </ul>
  </nav>
</aside>
<main>
  <h3>Main Content</h3>
  <p>This area shifts to make room for the sidebar.</p>
</main>
```
</div>

{% end %}
