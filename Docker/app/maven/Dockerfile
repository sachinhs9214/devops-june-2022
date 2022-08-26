FROM maven AS BUILD
WORKDIR /maven
COPY . /maven
COPY ./libraries /root/.m2
RUN cd ./target; ls
RUN mvn clean package -Dmaven.test.skip=true
