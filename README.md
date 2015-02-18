accessibility
===
##概要
moodleでページの文字サイズや背景を変更するプラグイン

##使い方
左下にACCESSIBILITYというブロックがあるのでそこのボタンを押せばサイズや色が変わる．  
Launch ATbarを押すと画面上部にメニューバーとして表示されるのでそこでも同様のことができる．

##Moodleのログインアカウント
name:test pass:Test_000

##WebDriver Tips
1.クリック  
driver.findElement(By.xpath("hoge")).click();  

2.ホバー    
// アクション：一連のイベントを作成  
Actions actions = new Actions(driver);    
// 移動先の要素を取得  
WebElement target = driver.findElement(By.xpath("hoge"));  
// ホバーイベントを登録  
actions.moveToElement(target);  
// アクション実行
actions.perform();  

3.リサイズ  
// 指定のウィンドウサイズに変更  
int width = 1000;  
int height = 500;  
driver.manage().window().setSize(new Dimension(width, height));  

// 最大化  
driver.manage().window().maximize();  
