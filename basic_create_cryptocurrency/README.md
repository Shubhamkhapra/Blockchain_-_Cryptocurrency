# Blockchain_-_Cryptocurrency
Step 1 :- To run hadcoin_node_5001.py & hadcoin_node_5002.py & hadcoin_node_5003.py on Pycharm 

step 2 :- select (Get method )on Postman to get blockchain 
					http://127.0.0.1:5001/get_chain
					http://127.0.0.1:5002/get_chain
					http://127.0.0.1:5003/get_chain
					
				select (POST Method) on postman
				http://127.0.0.1:5001/connect_node
				select body and next select to raw & JSON formate
				enter :-
				{
						"nodes": [
								"http://127.0.0.1:5002",
								"http://127.0.0.1:5003"
						]
				}
				
				Now blockchain are full connect to each node Decentralizing our blockchain
				
				Now select Get method on postman
				http://127.0.0.1:5001/mine_block
				Mine the block on blockchain
				
				now replace the original chain
				http://192.168.106.56:5003/replace_chain
				
				Now add the transactions of block
				Select the POST method on postman 
				http://192.168.106.56:5001/add_transaction
				and add to body of message on raw formate JSON
				{
					"sender": "Sk",
					"receiver": "Yash",
					"amount": 10000
				}
				
				pic
				
				Now mine the block to add this transaction on block
				http://192.168.106.56:5001/mine_block
				
				
					
