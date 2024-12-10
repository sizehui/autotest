# autotest

Browser based automated testing framework

## Installation

```
$ git clone https://github.com/bruceon/autotest.git
$ cd autotest
$ npm run build
```

The newly generated dist directory will be your working directory. Just follow the case example in dist/cases/sample to develop your own cases and place them in the dist/cases directory. Afterward, run the following commands to automatically execute all these cases:

```
$ cd dist
$ node autotest.js
```

## Usage

### Command-Line Arguments

You can get detailed usage information through the command-line arguments -h, --help or -?:

```
$ node autotest.js -h
```
<img src="data:image/png;base64,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" alt="Red dot" />
![]()

The -v option enables verbose mode, which is equivalent to setting `process.env.NODE_ENV="development"` during program execution. Alternatively, the same effect can be achieved by adding the following line to the `.env` file:

```
NODE_ENV='development'
```

The -c option is used to specify the target test cases to run. All test cases must be located in the cases directory, which is at the same level as the autotest.js file. Each JavaScript file in this folder and its subdirectories is treated as a test case. These test cases can be categorized by test projects and organized into different subfolders, with no limit on the number of folder levels.

The -c option can specify either a folder, in which case all test cases in that folder and its subdirectories will be run recursively, or a single JavaScript file, in which case only the specified test case will be executed.

### Configuration Files

There are two main configuration files, `.env` and `settings.js`, which must be placed in the same directory as `autotest.js` so that `autotest.js` can find them during startup. The `.env` file is used to set various environment variables. Currently, the environment variable required by the autotest framework is mainly `NODE_ENV`, which is used to distinguish between development mode and production mode. Different modes affect certain file path settings (related to VSCode IDE, the import() function in node.js, and Webpack's bundling process), and also influence the logging level of the logging tool, thereby affecting the corresponding log outputs.

For this project, the `NODE_ENV` variable essentially has three meaningful values: `"development"`, `"production"`, and `"IDE"`. The value of `NODE_ENV` should only be set to `"IDE"` when debugging the code in the VSCode IDE. In a real production environment, if necessary, you can still set `NODE_ENV` to `"development"`. This is useful for cases where unexpected behavior occurs at runtime, as it allows you to see more log information, making debugging easier.

Compared to the .env file, the settings.js file is more complex. This file mainly handles two aspects of configuration: one is related to the autotest framework itself, and the other is related to the logging tool. The part related to the test framework is as follows:

```
autotest: {
  headless: false,
  maxConcurrency: 10,
  // browserPath: 'C:\\Program Files\\Google\\Chrome\\Application\\chrome.exe',
  casesDir: process.env.NODE_ENV !== 'IDE' ? './cases' : './src/cases',
},
```

The first configuration option, `headless`, determines whether to use silent mode when running the test cases. The autotest framework is built on top of `Puppeteer`. If headless is set to true, `Puppeteer` will run without launching the browser's graphical interface. Otherwise, the browser will be opened. During development and debugging of test cases, setting this option to `false` is beneficial as it allows us to see the entire execution process of the case. However, in a production environment, setting it to `true` improves the execution efficiency of the test cases and is also easier for integrating the autotest framework into the DevOps pipeline.

The `maxConcurrency` option specifies how many parallel page instances you intend to launch to handle your test cases. In theory, the larger this option is set, the higher the concurrency and efficiency of the testing process. However, this also depends on the resource limitations of the runtime environment and the robustness of the system under test. Generally, setting this option to `10` is appropriate. You can adjust this value based on the specific conditions of your environment.

The `browserPath` option is related to the installation path of the browser. `Puppeteer` comes with a built-in `Chromium` browser. If you do not explicitly specify the `browserPath` parameter, the `autotest` framework will attempt to use `Puppeteer`'s built-in `Chromium` browser. However, the downside is that `Webpack` does not package the `Chromium` browser into the final `autotest.js` during the bundling process. As a result, if `autotest.js` is moved to somewhere outside the development environment for execution, you are highly likely to see the following error:

```
unhandledRejection: Could not find Chrome
```

In such cases, you need to set the `browserPath` option to the correct installation path of your Chrome. An example on windows goes like this:

```
browserPath: 'C:\\Program Files\\Google\\Chrome\\Application\\chrome.exe'
```

The directory structures in the IDE environment and the production environment are different. The `casesDir` option is used to inform the autotest framework which directory to retrieve test cases from in each environment. Keep it as is.

The majority of the remaining options in `settings.js` are related to `logging`. They have been carefully tuned, so just keep them as they are.

### Developing Cases

You can refer to the examples in cases/sample to develop your own test cases.

Test cases under the autotest framework have some basic requirements. First, you need to define and export a `config` object. An example of such an object is shown below:

```
export const config = {
  project: 'my_test_project',
  name: 'my_test_case',
  description: 'CRUD of devie type',
  entries: [
    {
      url: 'https://your-server/your-url',
    },
  ]
};
```

In this object, the properties `project`, `name`, `description`, and `entries` are mandatory, while the others are optional. The `entries` array must contain at least one item, and that item must include the `url` properties, which serves as the test entry point for the test case.

Additionally, you need to define a `run` function with the following signature:

```
export async function run(page, crawl, option) {
  ......
  const result = {
    case: {
      project: config.project,
      name: config.name,
      description: config.description,
      status: 'PASS' // maybe 'FAIL'
    }
  };
  ......

  return result;
}
```

The `run` function must return a `result` object as shown above. The parameters `page`, `crawl`, and `option` can be used to construct your test logic.

In the `run` function, you can reference your own utility functions or code. Simply define these in the `common` directory.

In the run function, you can use a logging tool provided by `autotest` to output any logs you need at any point:

```
this.logger.debug(`case ${config.name}: login successfully`);
......
this.logger.info(`case ${config.name}: result validated`);
......
this.logger.error(`case ${config.name}: failed to add device into the list`);
```

In the run function, you can utilize any features of `Puppeteer` as well as some utilities that `autotest` has already prepared for you:

```
// navigate to an element indicated by selector 'input[placeholder="请输入密码"]',
// focus on it, and input somthing
await input(page, 'input[placeholder="请输入密码"]', config.entries[0].auth.password)
```

```
// navigate to an element indicated by selector 'xpath/......',
// click on it,
// wait for the route to switch and the new page to fully load.
await click(page, `xpath/.//button[@type='button']/span/span[text()='登 录']`, true)
```

```
// navigate to an element indicated by selector 'xpath/......',
// click on it, (this will not trigger a route change)
await click(page, `xpath/.//span[text()='新增']`)
```

```
// retrieve the value of element indicated by selector 'tbody>......',
const deviceType = await page.$eval('tbody>tr:nth-child(1)>td:nth-child(2) span',
  (item) => item.textContent)
```

## License

MIT

## Acknowledgements

- [Puppeteer](https://github.com/puppeteer/puppeteer)
- [headless-chrome-crawler](https://github.com/yujiosaka/headless-chrome-crawler)
