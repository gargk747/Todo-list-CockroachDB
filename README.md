## Important note

Add the following header in a comment at the beginning of each source
file, and fill in your name and the year.

   Copyright [2020] [prantoran]

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.


Create [virtual env](https://docs.python.org/3/tutorial/venv.html) in the project directory
1. python3 -m venv tutorial-env
2. source tutorial-env/bin/activate

pip install psycopg2-binary

Setup CockRoachDB using docker
1. Install Docker
2. execute `./setup-database.sh install` or sequentially run the commands in that scripts which are acquired from the [Cockroach installation blog](https://www.cockroachlabs.com/docs/v20.1/start-a-local-cluster-in-docker-linux).


Run Flask server
export FLASK_APP=todo.py
flask run