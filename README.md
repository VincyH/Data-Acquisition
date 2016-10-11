# Data-Acquisition

##Abstract
this is data acquisition about battery , CPU , memory and memory leak is base on uiautomator or other UI automated test scripts that base on junit

##Usage

1、add the data.jar in your uiautomator project  
2、change your uiautomator TestCase code
   ```java
  private DataCollection dg
    
  protected void setUp() throws Exception {
		dg = DataCollection.getInstance();  
		super.setUp();
	   }
	
  protected void tearDown() throws Exception {
		 dg.dataGather(getName(), PackageName,ActivityName);
		 if (getName().equals("the last test name")) {
		 dg.drawPicture("your model name");
		 }
   ```

###Result
![github](https://github.com/VincyH/Data-Acquisition/blob/master/pic.jpg "github")  
