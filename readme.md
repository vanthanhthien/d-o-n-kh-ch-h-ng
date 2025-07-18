# setup và installation
```bash
#tạo môi trường ảo
python -m venv venv
#kích hoạt môi trường ảo
venv\Scripts\activate
#tải các tài nguyên cần thiết
pip install -r requirements.txt
#chạy ứng dụng
uvicorn app.main:app --reload

```

# ứng dụng sẽ chạy ở
- giao diện web: http://localhost:8000/
- API docs: http://localhost:8000/docs

# test api:
```bash
curl -X 'POST' \
  'http://localhost:8000/predict' \
  -H 'Content-Type: application/json' \
  -d '{
  "age": 35,
  "time_spent_on_site": 5.2,
  "pages_visited": 8,
  "previous_purchases": 2,
  "cart_value": 75.5,
  "is_returning_customer": 1,
  "days_since_last_visit": 7
}'
```

