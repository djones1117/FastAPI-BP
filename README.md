# Run Using...

uvicorn app:app --reload


# Test Using...

curl -X 'POST' \
  'http://127.0.0.1:8000/process_data' \
  -H 'accept: application/json' \
  -H 'Content-Type: application/json' \
  -d '{"data": "example input"}'


curl -X 'POST' \
  'http://127.0.0.1:8000/process_data_concurrent' \
  -H 'accept: application/json' \
  -H 'Content-Type: application/json' \
  -d '{"items": ["item1", "item2", "item3"]}'