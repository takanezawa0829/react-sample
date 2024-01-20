<!-- ビルド -->
docker-compose build
<!-- プロジェクトを作成 -->
docker-compose run --rm app sh -c 'npx create-react-app react-sample --template typescript'
<!-- プロジェクトの管理者をrootから変更 -->
sudo chown -R $USER:$USER /home/takane/Documents/react-sample/app/react-sample
<!-- コンテナ起動 -->
docker-compose up -d