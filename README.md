## Домашнее задание, вторая неделя:
Сделать свой блокчейн с единственным майнером в сети. См. видеоурок "Как сделать свой блокчейн за 200 строк кода"
Переработал пример - https://github.com/lhartikk/naivechain
1. Добавил proofs of work, в виде перебора хешей с нулями.
2. Добавил регулировку сложности - в нулевом блоке блокчейна выставлятся количество нулей в начале хеша.
3. Естественно пришлось дополнить верификацию блока и сам сблок новыми свойствами.
*****
### Установка
```
git clone https://github.com/svarog-vlz/bfm1.git
```
```
npm i
```
### Запуск

```
node index.js   
```
или
```
node index.js --notice
```
- для наблюдения за процессом майнинга
*****
Послать новый блок, получить список можно так-же как и в примере

#### Добавить блок 
```
curl -H "Content-type:application/json" --data '{"data" : "Some data to the first block"}' http://localhost:3001/mineBlock
```
#### Посмотреть блокчейн
```
curl http://localhost:3001/blocks
```
*****
2. ПО установил
3. Остальная часть ДЗ в папке transactions, с сылками на etherScan
