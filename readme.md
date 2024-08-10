# only use for release

# cài đặt các thư viện cần thiết cho client-app (Nextjs), win-app (application install on windows)
# build client-app với chế độ production (.env và .env.server)


# #####################################################
# cài đặt mongo window: https://www.mongodb.com/try/download/community
# cài đặt mongosh: https://www.mongodb.com/try/download/shell
# vào thư mục bin của mongo
# Setup replication
        # mongod.conf

        # for documentation of all options, see:
        #   http://docs.mongodb.org/manual/reference/configuration-options/

        # Where and how to store data.
        storage:
        dbPath: C:\Program Files\MongoDB\Server\7.0\data

        # where to write logging data.
        systemLog:
        destination: file
        logAppend: true
        path:  C:\Program Files\MongoDB\Server\7.0\log\mongod.log

        # network interfaces
        net:
        port: 27017
        bindIp: 127.0.0.1


        #processManagement:

        #security:

        #operationProfiling:

        #replication:
        replication:
        oplogSizeMB: 100
        replSetName: "rs0"
        enableMajorityReadConcern: true

        #sharding:

        ## Enterprise-Only Options:

        #auditLog:
# mở cmd và cd vào thư mục bin của mongo. Sau đó gõ lệnh: 
        # mongosh
        # rs.initiate()
        # set root user db.createUser({ user: "root", pwd: "123", roles: [ { role: "root", db: "admin" } ] })
        # db.grantRolesToUser( "root",[{ db: "main_win_icafe" }])



# Cài đặt redis
        # https://github.com/microsoftarchive/redis/releases

# Cài đặt npx
        # npm i -g npx
