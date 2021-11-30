# https://www.terraform.io/downloads.html

provider "aws" {
    region = "ap-northeast-1"
    access_key = "AKIAQIPNDBF5CSODPNMN"
    secret_key = "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"
}

resource "aws_iam_user" "IAMUser" {
    path = "/"
    name = "a-mori@cresco.co.jp"
    tags {
        Name = "a-mori@cresco.co.jp"
    }
}

resource "aws_iam_user" "IAMUser2" {
    path = "/"
    name = "h-akiyama@cresco.co.jp"
    tags {}
}

resource "aws_iam_user" "IAMUser2" {
    path = "/"
    name = "h-akiyama@c3w.co.jp"
    tags {}
}