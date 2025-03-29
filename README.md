# 🚀 보안 관제 시 차단하면 안 되는 공인 IP 목록

## 📌 개요
본 문서는 보안 관제 및 네트워크 운영 시 필수적인 공인 IP를 정리한 목록입니다.  
아래 IP들은 글로벌 서비스, 네트워크 인프라, DNS 및 주요 클라우드 서비스 제공자의 IP로,  
오인 차단 시 서비스 장애가 발생할 수 있습니다.

---

## 🌍 주요 글로벌 서비스 및 인프라 IP 목록

| IP 주소 | 제공자 | 설명 |
|---------|--------|------|
| `8.8.8.8` | Google | 공용 DNS (Primary) |
| `8.8.4.4` | Google | 공용 DNS (Secondary) |
| `1.1.1.1` | Cloudflare | 공용 DNS (Primary) |
| `1.0.0.1` | Cloudflare | 공용 DNS (Secondary) |
| `9.9.9.9` | Quad9 | 보안 강화 DNS |
| `208.67.222.222` | OpenDNS (Cisco) | 공용 DNS (Primary) |
| `208.67.220.220` | OpenDNS (Cisco) | 공용 DNS (Secondary) |

---

## ☁️ 클라우드 서비스 제공업체

| IP 주소 또는 대역 | 제공자 | 설명 |
|------------------|--------|------|
| `13.32.0.0/15` | AWS | CloudFront 서비스 |
| `35.190.0.0/17` | Google Cloud | Google 서비스 IP |
| `104.16.0.0/13` | Cloudflare | CDN 및 보안 서비스 |
| `172.217.0.0/16` | Google | Google 주요 서비스 (Gmail, YouTube 등) |
| `151.101.0.0/16` | Fastly | CDN 및 성능 최적화 서비스 |
| `185.199.108.0/22` | GitHub | GitHub Pages 및 서비스 IP |

---

## 🏛️ 주요 글로벌 플랫폼 IP

| IP 주소 또는 대역 | 제공자 | 설명 |
|------------------|--------|------|
| `13.35.0.0/16` | AWS | Amazon 서비스 |
| `157.240.0.0/16` | Meta (Facebook) | Facebook 및 WhatsApp |
| `185.60.216.0/22` | WhatsApp | WhatsApp 서비스 |
| `204.79.197.200` | Microsoft | Bing 검색 서비스 |
| `17.0.0.0/8` | Apple | Apple iCloud 및 서비스 |

---


글로벌 플랫폼 ip는 변경 가능성 있음 (유동적임 dhcp protocol)
## ⚠️ 주의 사항
- 위 목록은 대표적인 IP만 포함하며, 해당 업체의 공식 문서를 통해 최신 정보를 확인해야 합니다.
- 보안 정책 적용 시, 필수 IP 차단 여부를 반드시 검토해야 합니다.

---

### 📄 참고 자료
- [Google Public DNS](https://developers.google.com/speed/public-dns)
- [Cloudflare Public DNS](https://1.1.1.1/)
- [Quad9 Security DNS](https://www.quad9.net/)
- [AWS IP Ranges](https://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html)
- [Google IP Ranges](https://support.google.com/a/answer/60764)
- [GitHub IP Ranges](https://api.github.com/meta)
