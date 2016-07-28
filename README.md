# Data-Acquisition

##Abstract
this is data acquisition about battery , CPU , memory and memory leak is base on uiautomator(1.0 or 2.0) automated test scripts

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
![github](http://github.com/unicorn.png "github")  
