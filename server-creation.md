# Server Creation

Stellar Bit is a community driven game. People can create their own servers with customized objectives and features.

There are two types of servers a person can create. Either a publicly hosted one accessible by anyone with the official Stellar Bit account or private without authorization capabilities.

## Public server

You will need to have an official Stellar Bit account, which you can create for free at https://stellar-bit.com.

Then on the webpage under the section `My Servers` click the plus button in the bottom right, to create your own server. Adjust the name and description as needed.

Now the server is offline. The server will be online only when keep-alive packets along with IPV4 address where others can access it are being sent to the Stellar Bit Hub every 5 minutes.

To simplify the process there is already a template created at https://github.com/stellar-bit/server-template-auth.

To run the template with its default logic (which you can adjust later) on your machine follow these steps:
1. Download the template repository 
2. Open the template folder in your code editor
3. Adjust the constants `SERVER_ADDR` and `SERVER_NAME` in `src/lib.rs` as needed
4. Run the server using `cargo r --release`
5. Enter your Stellar Bit account credentials
6. Potentially test the connection through some client

## Private server

Similar to public server.

You can use the template at https://github.com/stellar-bit/server-template.

In the template folder you can adjust `SERVER_ADDR` in `src/lib.rs` as needed.

Run by executing `cargo r --release`.



## Server logic

TODO




