FROM python:3.8

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY business_logic_service.py .
COPY static static/
COPY templates templates/

EXPOSE 5001

CMD ["python", "business_logic_service.py"]
