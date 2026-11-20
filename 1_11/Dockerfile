from maven:3.8.6-amazoncorretto-8 as build

workdir /usr/src/app

copy . . 

run mvn clean package

from amazoncorretto:8

workdir /usr/src/app

copy --from=build /usr/src/app/target/*.jar app.jar

expose 8080

cmd ["java", "-jar", "app.jar"]
