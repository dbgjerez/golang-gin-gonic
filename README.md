# POC Gin Gonic

# Installation
* Use a vendor like govendor: https://github.com/kardianos/govendor
    * set $GOPATH and $PATH variables (if you have not it)
    ```bash
        echo "export $GOPATH=$HOME/go" >> ~/.bashrc
        echo "export $PATH=$GOPATH/bin:$PATH" >> ~/.bashrc
        source ~/.bashrc
    ```
    * install govendor
    ```bash
        go get github.com/kardianos/govendor
    ```

# How to create first demo application
* Create, clone or link the project and ```cd``` inside
    * Create  
    ```bash
        mkdir -p $GOPATH/src/github.com/myusername/project && cd "$_"
    ```
    * Clone
    ```bash
        git clone "github.com/myusername/project" $GOPATH/src/github.com/myusername
    ```
    * Link
    ```bash
        ln -s $PROJECT_HOME $GOPATH/src/github.com/myusername 
        cd $PROJECT_HOME
    ```
* Init the project using govendor
    ```bash
        govendor init
        govendor fetch github.com/gin-gonic/gin@v1.3
    ```
* Copy an example template
    ```bash
    	curl https://raw.githubusercontent.com/gin-gonic/examples/master/basic/main.go > main.go
    ```
* Run the project
    ```bash
    	go run main.go
    ```
