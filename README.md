# 振り返り

今回の課題に使った参考サイトや、課題になったことなどを網羅的に記録しています

## 目標

> React チュートリアルを関数コンポーネントで実装する。

参考サイト: [React チュートリアルを関数コンポーネントで書き換えてみた](https://nishinatoshiharu.com/functional-react-tutorial/)

## 記録

-   公式チュートリアルもそうだが、コンポーネントごとにファイルを分けて記述していないため実践とは少し違うため、煩わしかった。せっかくならコンポーネントごとにファイルを分けたコードが知りたかった
    -   自分でそのコードをかけたので、ちょうどいい難易度だったのかも？
-   React チュートリアルはいくつかの手順に分けられていますが、その中でも「手番の処理」あたりまでは比較的順調に進んだ。
-   handleClick のリフトアップや calculateWinner が複数コンポーネントで使う点に戸惑いを感じた。
-   りあクトの熟読のおかげで React の基本理念がわかっていたため、りあクトの復習、参考サイトの熟読でほとんどのエラーを解決できた
-   JavaScript の知らないメソッドに解読を悩まされることが多かった。
    -   slice()
    -   current  
        は見慣れなかった。まだよくわかっていない

## チュートリアルを通してわかったこと

-   props の渡し方は二つあるが、props を記述する方法がわかりやすい。

    -   理由はそのコンポーネントの変数なのか親コンポーネントに渡したい props なのか見分けがつきにくいから

    ```
       const something = (props) =>{
            //コンポーネント
             <div> {props.text} </div>
            }
    ```

    ```
    const something ( {text} ) =>{
        // コンポーネント
        <div> {text} </div>
    }
    ```

-   コードは写経してもいいので、自分の手で打つことが大事。
    -   コピペだとどうしても細かい部分にまで、目がいかないので、上達速度に違いが出ると思う
-   関数コンポーネントへの変換や const での関数宣言を積極的に取り入れ、モダンなコードの書き方を身につけていくべき。
    -   いくつかの参考サイトを見たが、クラスコンポーネントや function での関数宣言をしているサイトが多かったが、日頃から「よりモダンな、より安全なコードを実現するためにはどうしよう」とたまに思い返してみることでコーディングは上達すると思った。

---

以下、初期の README

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `yarn build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
