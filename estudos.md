1° Iniciar o ambiente virtual > "python -m venv venv" - Para iniciar a venv -> "./venv/Scripts/activate.ps1"

2° instalar o django > "pip install Django"

3° instalar o dotenv > pip install python-dotenv"

4° criar lista com todas as dependencias > "pip freeze > requirements.txt" - lembrar de semore atualizar quando adicinar alguma dependencia

5° iniciar o servidor > "django-admin startproject setup ."

APP é um pedaço de aplicação que possui alguma funcionalidade no Django
Projeto é a coleçao de todoas a configurações em uma aplicação. Um projeto pode conter diversos apps dentro dele

6° Para iniciar um app > "python manage.py startapp nome_do_app"

7° configurar os urls do novo app

8° configurar o arquivo de views do app

9° configurar os Statics file dir no setting de setup e criar a pasta static dentrode setup

STATISFILES_DIR = [
    os.path.join(BASE_DIR, 'setup/static')  `todos os arquivos estáticos estão dsentro dessa pasta`
]

STATIC_ROOT = os.path.join(BASE_DIR, 'static') `caminho absluto para o diretório onde o python vai coletar esses arquivos para fazer a implementação`

Depois passar os arquivos css e a pasta assets para a pasta static

10° Rodar o comando "python manage.py collectstatic" faz o endereçamento para o django pegar eles

11° arrumar o caminho para os links no arquivo html
