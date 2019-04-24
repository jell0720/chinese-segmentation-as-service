# chinese-segmentation-as-service

Using `Flask` export `jieba`/`SnowNLP`/`pkuseg` as http API web service.

## require

1. python 3.7 (`$ brew install python3`)
2. pipenv (`$ brew install pipenv`)

## Usage

1. clone it `$ git clone https://github.com/jk195417/chinese-segmentation-as-service.git`
2. `$ cd chinese-segmentation-as-service`
3. `$ pipenv update`
4. `$ pipenv run python app.py`, serve on http://localhost:3001
5. `$ curl -X POST -H "Content-Type: application/json" -d '{"text" : "要斷詞的文字"}' "http://localhost:3001/segmentations"`
