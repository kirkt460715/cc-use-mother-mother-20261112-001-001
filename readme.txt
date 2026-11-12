County cohort and school capacity analysis. Bundled records are synthetic.
Python 3.11 or later; standard library only.
Demo: python3 cohort_cli.py demo --fixture fixtures/county.json
Tests: python3 -m unittest discover -s tests -v
Build: python3 -m compileall -q cohorts forecast school_pressure releases cohort_cli.py
Portfolio: python3 cohort_cli.py portfolio fixtures/county.json --baseline baseline
Quality: python3 cohort_cli.py audit fixtures/county.json
Run: python3 cohort_cli.py run fixtures/county.json --database /tmp/cohorts.sqlite3 --scenario baseline --request-key county-baseline
API: python3 cohort_cli.py serve --database /tmp/cohorts.sqlite3 --host 127.0.0.1 --port 8080
Other commands: python3 cohort_cli.py --help
