# fatmah

from datetime import date

# Customer Class
class Customer:
    def __init__(self, customer_id, name, email, phone_number, address, password):
        self.customer_id = customer_id
        self.name = name
        self.email = email
        self.phone_number = phone_number
        self.address = address
        self.password = password
    
    def set_customer_id(self, customer_id): self.customer_id = customer_id
    def get_customer_id(self): return self.customer_id
    def set_name(self, name): self.name = name
    def get_name(self): return self.name
    def set_email(self, email): self.email = email
    def get_email(self): return self.email
    def set_phone_number(self, phone_number): self.phone_number = phone_number
    def get_phone_number(self): return self.phone_number
    def set_address(self, address): self.address = address
    def get_address(self): return self.address

# Order Class
class Order:
    def __init__(self, order_id, order_date, customer, status, subtotal, taxes, total_amount, discount_applied):
        self.order_id = order_id
        self.order_date = order_date
        self.customer = customer
        self.status = status
        self.subtotal = subtotal
        self.taxes = taxes
        self.total_amount = total_amount
        self.discount_applied = discount_applied
    
    def set_order_id(self, order_id): self.order_id = order_id
    def get_order_id(self): return self.order_id
    def set_order_date(self, order_date): self.order_date = order_date
    def get_order_date(self): return self.order_date
    def set_status(self, status): self.status = status
    def get_status(self): return self.status
    def set_subtotal(self, subtotal): self.subtotal = subtotal
    def get_subtotal(self): return self.subtotal
    def set_taxes(self, taxes): self.taxes = taxes
    def get_taxes(self): return self.taxes

# Product Class
class Product:
    def __init__(self, product_id, product_name, price, stock_availability, category, weight):
        self.product_id = product_id
        self.product_name = product_name
        self.price = price
        self.stock_availability = stock_availability
        self.category = category
        self.weight = weight
    
    def set_product_id(self, product_id): self.product_id = product_id
    def get_product_id(self): return self.product_id
    def set_product_name(self, product_name): self.product_name = product_name
    def get_product_name(self): return self.product_name
    def set_price(self, price): self.price = price
    def get_price(self): return self.price
    def set_stock_availability(self, stock_availability): self.stock_availability = stock_availability
    def get_stock_availability(self): return self.stock_availability
    def set_category(self, category): self.category = category
    def get_category(self): return self.category

# Payment Class
class Payment:
    def __init__(self, payment_id, amount, method, credit_card_number, cvv, transaction_status, payment_date, invoice_number):
        self.payment_id = payment_id
        self.amount = amount
        self.method = method
        self.credit_card_number = credit_card_number
        self.cvv = cvv
        self.transaction_status = transaction_status
        self.payment_date = payment_date
        self.invoice_number = invoice_number
    
    def set_payment_id(self, payment_id): self.payment_id = payment_id
    def get_payment_id(self): return self.payment_id
    def set_amount(self, amount): self.amount = amount
    def get_amount(self): return self.amount
    def set_method(self, method): self.method = method
    def get_method(self): return self.method

# DeliveryStaff Class
class DeliveryStaff:
    def __init__(self, staff_id, name, phone_number, delivery_status, vehicle_type, location):
        self.staff_id = staff_id
        self.name = name
        self.phone_number = phone_number
        self.delivery_status = delivery_status
        self.vehicle_type = vehicle_type
        self.location = location
    
    def set_staff_id(self, staff_id): self.staff_id = staff_id
    def get_staff_id(self): return self.staff_id
    def set_name(self, name): self.name = name
    def get_name(self): return self.name
    def set_phone_number(self, phone_number): self.phone_number = phone_number
    def get_phone_number(self): return self.phone_number

# Delivery Class
class Delivery:
    def __init__(self, delivery_id, order, delivery_date, estimated_arrival, tracking_number, current_status, delivery_method):
        self.delivery_id = delivery_id
        self.order = order
        self.delivery_date = delivery_date
        self.estimated_arrival = estimated_arrival
        self.tracking_number = tracking_number
        self.current_status = current_status
        self.delivery_method = delivery_method
    
    def set_delivery_id(self, delivery_id): self.delivery_id = delivery_id
    def get_delivery_id(self): return self.delivery_id
    def set_delivery_date(self, delivery_date): self.delivery_date = delivery_date
    def get_delivery_date(self): return self.delivery_date

# Admin Class
class Admin:
    def __init__(self, admin_id, name, email, phone_number, password, role):
        self.admin_id = admin_id
        self.name = name
        self.email = email
        self.phone_number = phone_number
        self.password = password
        self.role = role
    
    def set_admin_id(self, admin_id): self.admin_id = admin_id
    def get_admin_id(self): return self.admin_id
    def set_name(self, name): self.name = name
    def get_name(self): return self.name
    def set_email(self, email): self.email = email
    def get_email(self): return self.email
