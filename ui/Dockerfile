FROM klakegg/hugo:0.43-ext-alpine

# Get git
RUN apk add --update git

# Copy script and allow execution
COPY ./build-static-site.sh /build-static-site.sh
RUN chmod 0777 /build-static-site.sh

ENTRYPOINT ["sh", "/build-static-site.sh"]
