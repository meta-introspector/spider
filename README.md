# Spider

Web spider framework that can spider a domain and collect pages it visits.

## Depensencies

~~~bash
$ apt install openssl libssl-dev
~~~

## Usage

## from source for command line usages

~~~bash
$ git clone https://github.com/madeindjs/spider.git
$ cd spider
$ cargo build --release
$ ./target/debug/rust-crawler # TODO: parse command line arguments
~~~

## as crate for librairy usage

Add this dependency to your _Cargo.toml_ file.

~~~toml
[dependencies]
TODO
~~~

## Use

~~~rust
// insert crate here

let mut localhost = Website::new("http://localhost:4000");
localhost.crawl();

for page in localhost.get_pages() {
    println!("- {}", page.get_url());
}

// TODO
~~~


## TODO

- [ ]: multi-threaded system
- [ ]: respect _robot.txt_ file
- [ ]: add configuratioon object for polite delay, etc..
- [ ]: parse command line arguments

## Contribute

I am open-minded to any contribution. Just fork & `commit` on another branch.


