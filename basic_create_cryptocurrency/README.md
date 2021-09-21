# Blockchain_-_Cryptocurrency

## ⚡ Step 1 :- 
```python
- To create Decentralizing network we are using Pycharm to run this code
- To run this file  hadcoin_node_5001.py & hadcoin_node_5002.py & hadcoin_node_5003.py on Pycharm 
```
![1.png](https://github.com/Shubhamkhapra/Blockchain_-_Cryptocurrency/blob/b8cdd635fa5c21b7e0c9079fd281ca9c5bc160c6/img/1.png)

## ⚡ Step 2 :- 
```python
- select (Get method )on Postman to get Chain  
	http://127.0.0.1:5001/get_chain
	http://127.0.0.1:5002/get_chain
	http://127.0.0.1:5003/get_chain
```
![2.png](https://github.com/Shubhamkhapra/Blockchain_-_Cryptocurrency/blob/b8cdd635fa5c21b7e0c9079fd281ca9c5bc160c6/img/2.png)

## ⚡ Step 3 :- 
```python
- Select (POST Method) on postman to connect full chain
	1. http://127.0.0.1:5001/connect_node
		select body and next select to raw & JSON formate
			enter :-
				{
				  "nodes": [
						"http://127.0.0.1:5002",
						"http://127.0.0.1:5003"
					   ]
				}
				
	2. http://127.0.0.1:5002/connect_node
		select body and next select to raw & JSON formate
			enter :-
				{
				  "nodes": [
						"http://127.0.0.1:5001",
						"http://127.0.0.1:5003"
					   ]
				}
	3. http://127.0.0.1:5003/connect_node
		select body and next select to raw & JSON formate
			enter :-
				{
				  "nodes": [
						"http://127.0.0.1:5001",
						"http://127.0.0.1:5002"
					   ]
				}
				
	Now blockchain are full connect to each node Decentralizing  network our blockchain
```
![3.png](https://github.com/Shubhamkhapra/Blockchain_-_Cryptocurrency/blob/b8cdd635fa5c21b7e0c9079fd281ca9c5bc160c6/img/3.png)

## ⚡ Step 4 :- 
```python
- Select Get method on postman to mine new block 
	http://127.0.0.1:5001/mine_block
```
![4.png](https://github.com/Shubhamkhapra/Blockchain_-_Cryptocurrency/blob/b8cdd635fa5c21b7e0c9079fd281ca9c5bc160c6/img/4.png)

## ⚡ Step 5 :- 
```python
- Now check the block chain if some one add a new block or some one tempared  on blockchain 
	http://192.168.106.56:5003/replace_chain
	http://192.168.106.56:5002/replace_chain
```
![5.png](https://github.com/Shubhamkhapra/Blockchain_-_Cryptocurrency/blob/b8cdd635fa5c21b7e0c9079fd281ca9c5bc160c6/img/5.png)

## ⚡ Step 6 :- 
```python
- Now add create some transactions this transactions is add on Mempool on bitcon
	Select the POST method on postman 
	http://192.168.106.56:5001/add_transaction
		Select body add to body of message on raw formate JSON
				{
					"sender": "Sk",
					"receiver": "Yash",
					"amount": 10000
				}
```
![6.png](https://github.com/Shubhamkhapra/Blockchain_-_Cryptocurrency/blob/b8cdd635fa5c21b7e0c9079fd281ca9c5bc160c6/img/6.png)

## ⚡ Step 7 :- 
```python
- Now mine the new block to add this transaction on block
	http://192.168.106.56:5001/mine_block
```
![7.png](https://github.com/Shubhamkhapra/Blockchain_-_Cryptocurrency/blob/b8cdd635fa5c21b7e0c9079fd281ca9c5bc160c6/img/7.png)

## ⚡ Step 8 :- 
```python
- To Get full chain on blockchain using this on postman 
	http://192.168.106.56:5001/get_chain
```				
				
					
