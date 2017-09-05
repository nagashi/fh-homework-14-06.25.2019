# Homework 14 - Building gRPC client Part 2

## Due Date

TBD

## Goals

- The purpose of this homework is to extend Homework #13 by implementing
  a Ruby gRPC client.

## Readings and Resources

GRPC - https://grpc.io

Ruby gRPC Quick Start - http://www.grpc.io/docs/quickstart/ruby.html

Option Parser - https://ruby-doc.org/stdlib-2.1.1/libdoc/optparse/rdoc/OptionParser.html

Ruby Language - http://www.ruby-lang.org/en/documentation/

## Setup

  - Create feature branch

    $ cd homework-13
    $ git checkout -b part-02-ruby-grpc-client

    Note: You'll be building off the code from Part (1).

  - Change to working directory

    ```
    $ cd start
    ```

  - Start The Server

    ```
    $ node server.js
    ```

  - Create Gemfile

    ```
    $ touch Gemfile
    ```

  - Required Gems

    - add required gems to your gem file

      ```
      gem 'grpc', '~> 1.2.5'
      ```

  - Create Ruby client file

    ```
    $ touch client.rb
    ```

    Note:  You'll be adding your Ruby code to client.rb.

  - Writing the gRPC Client

    - complete step (9) of the following using the Ruby language:

      https://codelabs.developers.google.com/codelabs/cloud-grpc/index.html

    - command line interface (CLI)

      a) list

        ```
        $ ruby client.rb list
        ```

      b) insert

        ```
        $ ruby client.rb insert 2 "The Three Musketeers" "Alexandre Dumas"
        ```

      c) delete

        ```
        $ ruby client.rb delete 123
        ```

      d) list

        ```
        $ ruby client.rb list
        ```

      e) retrieve

        ```
        $ ruby client.rb get 2
        ```

      Note:  Your responses should be equal to the responses received from the
             Node client.  Also, please see the `Option Parse` reference for
             assisting with the building of your command line interface (CLI).

## Deliverables

  - push changes to Github

    ```
    $ git checkout part-02-ruby-grpc-client
    $ git push
    ```

  - merge changes into the master branch and push to Github

    ```
    $ git checkout master
    $ git merge part-02-ruby-grpc-client
    $ git push
    ```

## Have Questions

Please make a reasonable effort to complete the homework prior to our next session.  If you have any questions regarding this homework, please do send me a message via Slack.
