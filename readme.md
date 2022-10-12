<!-- GETTING STARTED -->
### Prerequisites

- Register to get the API token key -  [https://www.weatherbit.io/account/create](https://www.weatherbit.io/account/create)
- install Java and [download Jmeter](https://jmeter.apache.org/download_jmeter.cgi)

### Installation
1. Register to get the API token key -  [https://www.weatherbit.io/account/create](https://www.weatherbit.io/account/create)
2. Clone the repo
   ```sh
   git clone https://github.com/ardhi2015/jmeter-github-action
   ```
3. go to {your directory}/apache-jmeter-5.5/bin
4. open jmeter GUI
- use terminal and using following comand ./jmeter.sh (linux/mac os)
- double click jmeter.bat (windows)
5. change value`s API_KEY on 'User Defined Variables' to your API token

### How to run
1. open terminal
2. go to {your directory}/apache-jmeter-5.5/bin
3. Enter following command, jmeter -n –t test.jmx -l testresults.jtl
-n: It specifies JMeter is to run in non-gui mode
-t: Name of JMX file that contains the Test Plan
-l: Name of JTL(JMeter text logs) file to log results
-j: Name of JMeter run log file

### How to Generate HTML Report
1. go to {your directory}/apache-jmeter-5.5/bin
2. click Tools
3. click Generate HTML Report
4. input some item
 - Result file : JMeter run log file
 - user.properties.file (usualy in apache-jmeter-5.5/bin) 
 - output directory: empity folder directory
5. click generate html report
6. go to your output directory
7. there's html file report

### How to Trigger CI (Github Action)
push something to master