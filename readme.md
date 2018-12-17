//tutorial start
https://jojoldu.tistory.com/251?category=635883

//boot run cmd with gradle
With the configuration you have this should work:
./gradlew bootRun -Dserver.port=8090
With this piece of code:
bootRun {
   systemProperties = System.properties
}

//h2 default url
jdbc:h2:mem:testdb

//url test httpie
http POST localhost/posts title="test 제목2" content="test 내용2" author="test 글쓴이2"
