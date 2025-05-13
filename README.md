# GitOps Register App

Đây là một ứng dụng demo được triển khai theo mô hình GitOps sử dụng Argo CD trên Kubernetes.

## 📁 File trong repo

- `deployment.yaml`: Khai báo Deployment cho ứng dụng NGINX
- `service.yaml`: Tạo Service kiểu LoadBalancer để expose ứng dụng
- `README.md`: Mô tả project

## 🚀 Hướng dẫn sử dụng

### Bước 1: Clone repo
```bash
git clone https://github.com/<your-username>/gitops-register-app.git
cd gitops-register-app

##Apply thủ công (nếu không dùng ArgoCD)
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
