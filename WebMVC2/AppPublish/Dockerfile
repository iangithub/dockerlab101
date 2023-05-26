#See https://aka.ms/customizecontainer to learn how to customize your debug container and how Visual Studio uses this Dockerfile to build your images for faster debugging.

#Depending on the operating system of the host machines(s) that will build or run the containers, the image specified in the FROM statement may need to be changed.
#For more information, please see https://aka.ms/containercompat

FROM mcr.microsoft.com/dotnet/aspnet:6.0 AS base

#設定工作目錄
WORKDIR /APP

# 將專案 DLL 檔複製到工作目錄
COPY ./APP .

EXPOSE 80
EXPOSE 443

ENTRYPOINT ["dotnet", "WebMVC.dll"]