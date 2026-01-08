# بنستخدم صورة كالي الرسمية كأساس
FROM kalilinux/kali-rolling:latest

# تحديث النظام وتثبيت الأدوات (دي هتتنفذ مرة واحدة بس وقت البناء)
RUN apt-get update && apt-get upgrade -y && \
    apt-get install -y curl wget git gnupg build-essential python3-pip \
    nmap sqlmap hydra john ffuf dirb wpscan set && \
    apt-get clean && rm -rf /var/lib/apt/lists/*
    
