<div align="center">

## lustre_gleam_routing_test


####  Proof of concept of the `Modem` library for Lustre application routing (deployment on GitHub Pages hash-based routing)

<br /><br />

![GitHub License](https://img.shields.io/github/license/emarifer/routing_test) ![Static Badge](https://img.shields.io/badge/Gleam-%3E=1.13.0-ffaff3) ![Static Badge](https://img.shields.io/badge/Lustre%20framework-%3E=5.4.0-ffaff3) ![Static Badge](https://img.shields.io/badge/Erlang/OTP-%3E=27-B83998)

</div>

---

### 🚀 Features


**Routing with Lustre**, a web application (`SPA`) written in `Gleam` that uses the `Lustre` framework, with routing handled by the `Modem` library for Lustre. The main features of the framework are tested, especially its functional approach to the frontend within the [`Elm`](https://guide.elm-lang.org/architecture/) architecture and the [`Modem`](https://hexdocs.pm/modem/index.html) library, but with route matching modified to support [`hash routing`](https://dev.to/mktcode/github-pages-with-dynamic-routes-dli) (also known as `HashRouter` in the `React` world), since the deployment is on `GitHub Pages`, which uses a server that does not support dynamic routing for SPAs.

---

### 👨‍🚀 Getting Started

You can try the app [here](https://emarifer.github.io/routing_test/).

- <ins>Working on the code:</ins>

    With Gleam installed as explained [here](https://gleam.run/getting-started/installing/) (and `Erlang` and its `BEAM VM`), you only need to run the following command in a terminal open in the project folder to start the application in development mode:

    ```sh
    gleam add --dev lustre_dev_tools  
    ```

    This will download the dependencies, compile the project, and start a development server. In your browser, go to [http://localhost:1234](http://localhost:1234) and you will be able to see the application. Any changes you make to the code using your text editor will cause the browser to reload and display the changes.

    > The [lustre_dev_tools](https://hexdocs.pm/lustre_dev_tools/index.html) development server watches your filesystem for changes to your gleam code and can automatically reload the browser. For `Linux` users, this requires [inotify-tools](https://github.com/inotify-tools/inotify-tools) be installed. If you do not or cannot install this, the development server will still run but it will not watch your files for changes.

- <ins>Compiling the code for production deployment:</ins>

    If, after making changes to the code, you decide to test the `SPA application` on a `static file server`, simply run the following command in the project folder opened in a terminal:

    ```sh
    gleam run -m lustre/dev build routing_test --minify
    ```

    This will compile (or rather transpile) the `JavaScript` project, generating an `HTML` skeleton and minifying both the `CSS` and JavaScript files, saving everything in a `/dist` folder at the project root. You can find more details about configuring the build for development and production [here](https://hexdocs.pm/lustre/index.html) and [here](https://hexdocs.pm/lustre_dev_tools/index.html).

---

### 📚 Learn more

* Official website: https://gleam.run/
* Guides: https://hexdocs.pm/gleam_stdlib/index.html
* Lustre framework: https://hexdocs.pm/lustre/index.html
* Lustre Dev Tools: https://hexdocs.pm/lustre_dev_tools/index.html
* Community: https://discord.com/invite/Fm8Pwmy
* Gleam discussions on Github: https://github.com/gleam-lang/gleam/discussions

---

### Happy coding 😀!!
