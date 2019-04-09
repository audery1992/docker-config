FROM centos:7
ENV LANG C.UTF-8
WORKDIR /opt/hexo
RUN yum install -y git epel-release
RUN yum install -y nodejs && npm config set registry https://registry.npm.taobao.org \
&& npm install hexo-cli -g && hexo init judith && cd judith && npm install
WORKDIR judith
RUN npm install --save hexo-deployer-git
RUN git config --global user.email "1451203598@qq.com"
RUN git config --global user.name "audery1992"
#RUN chmod -R 777 /opt/hexo/judith
EXPOSE 4000
ENTRYPOINT ["hexo","server"]
