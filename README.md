# docusaurus-easy
아주 쉽게 도큐사우루스 문서 시스템을 만들수 있는 기본 템플릿 저장소

## CNAME 파일 생성

꼭 자신의 CNAME 파일에 커스텀도메인 주소를 넣어두기 바란다. 푸시할때 마다 없어진다.
github Acions 파일에 deploy 에 cname 옵션을 추가한다.

```
      # Popular action to deploy to GitHub Pages:
      # Docs: https://github.com/peaceiris/actions-gh-pages#%EF%B8%8F-docusaurus
      - name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          # Build output to publish to the `gh-pages` branch:
          publish_dir: ./build
          cname: 여기에원하는도메인명추가
```
