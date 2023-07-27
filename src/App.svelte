<main>
  <h1>Vite Build Variables Example</h1>
  <p>
    Vite <a
      href="https://vitejs.dev/guide/env-and-mode.html#production-replacement"
      >replaces <kbd>.env</kbd> variables</a
    >
    during the build process. This can be configured in
    <a style="color:#17f215" href="https://dappling.network">dAppling</a> as such:
  </p>
  <img
    src="/build-variables.png"
    style="height: 400px"
    alt="build variables example dAppling"
  />
  <p>
    For example, putting <kbd>{`{import.meta\u200b.env.VITE_CAT}`}</kbd> in your
    code will be replaced with <kbd>Meow!</kbd>.
  </p>
  <pre>
    {`<h1 style="color: orange">🐈 {import.meta\u200b.env.VITE_CAT}</h1>
  <h1 style="color: blue">🐶 {import.meta\u200b.env.VITE_DOG}</h1>`}
  </pre>
  <h1 style="color: orange">🐈 {import.meta.env.VITE_CAT}</h1>
  <h1 style="color: blue">🐶 {import.meta.env.VITE_DOG}</h1>
</main>
