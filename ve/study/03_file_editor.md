# 03 file editor

vue.config.js에 설정을 넣어준다.

아래의 코드가 기본코드이다.

``` js
pluginOptions: {
    electronBuilder: {
        builderOptions: {
            appId: 'com.DS.ve_test' //식별자,
            nsis: {
                shortcutName: 'Digital Study Bible'
            },
            win: {
                target:[
                    {
                        target: "nsis",
                        arch: [
                            'x64',
                            'ia32'
                        ]
                    }
                ]
            }
        }
    }
  }
```