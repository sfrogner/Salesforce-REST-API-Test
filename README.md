# Couple things to get this working.

1. Have a SFDC Developer or Enterprise Edition
2. Install Java (I used 1.7)
3. Install eClipse
4. Install Http Client (Used Apache)
      * http://hc.apache.org/downloads.cgi
      * 4.5tar.g
      * Uncompress in a folder
5. Install JSON framework
      * http://mvnrepository.com/artifact/org.json/json
      * Download 20140107 (You could try 20141113 with Java 8 if want to)
6. Created connected App in SFDC.  Goto Setup -> Create -> Apps.  Bottom of pag click New
      * Connected App Name = Test REST API
      * API Name = TEST_REST_API
      * Contact Email = Email
      * Click Enable OAuth Setting = True
      * Callback URL = https://localhost:8443/callback
      * Selected OAuth Scopes = Full Access(full)
      * Click SAVE
      * Click Continue
      * Note, You will need Consumer Key.  Click Consumer Secret and note key also.
7. Clone Rep
8. Add External Jars to build path
Connected App Name = Test REST API
      * httpclient "<version>"
      * httpcore-<version>
      * commons-logging-<version>
      * commons-codec-<version>
      * json-20141113.jar
      
Have fun
