---
title: "Update Category Tree"
slug: "updatecategorytree"
excerpt: ">📘 This API is part of the [Seller Portal Catalog](https://help.vtex.com/en/tutorial/how-the-seller-portal-catalog-works--7pMB6YOt6YQDQQbzFB4Pxp). This functionality is in the Beta stage and can be discontinued at any moment at VTEX's discretion. VTEX will not be responsible for any instabilities caused by its use or discontinuity. If you have any questions, please contact [our Support Center](https://support.vtex.com/hc/en-us/requests). \r\n\r\n Updates the existing categories in the category tree.\r\n\r\n## Request body example\r\n\r\n```json\r\n{\r\n  \"roots\": [\r\n    {\r\n      \"value\": {\r\n        \"id\": \"2\",\r\n        \"name\": \"Departamento Artesanato\",\r\n        \"isActive\": true\r\n      },\r\n      \"children\": [\r\n        {\r\n          \"value\": {\r\n            \"id\": \"3\",\r\n            \"name\": \"Artesanato de Barro\",\r\n            \"isActive\": false\r\n          },\r\n          \"children\": [\r\n            {\r\n              \"value\": {\r\n                \"id\": \"4\",\r\n                \"name\": \"Artesanato de Barro Vermelho\",\r\n                \"isActive\": false\r\n              },\r\n              \"children\": []\r\n            }\r\n          ]\r\n        }\r\n      ]\r\n    },\r\n    {\r\n      \"value\": {\r\n        \"id\": \"5\",\r\n        \"name\": \"Perfumes\",\r\n        \"isActive\": false\r\n      },\r\n      \"children\": [\r\n        {\r\n          \"value\": {\r\n            \"id\": \"6\",\r\n            \"name\": \"Perfume Feminino\",\r\n            \"isActive\": false\r\n          },\r\n          \"children\": []\r\n        },\r\n        {\r\n          \"value\": {\r\n            \"id\": \"7\",\r\n            \"name\": \"Perfume Masculino\",\r\n            \"isActive\": false,\r\n            \"displayOnMenu\": false,\r\n            \"score\": 0,\r\n            \"filterByBrand\": false,\r\n            \"isClickable\": false\r\n          },\r\n          \"children\": []\r\n        }\r\n      ]\r\n    }\r\n  ]\r\n}\r\n```"
hidden: false
createdAt: "2021-07-05T14:05:36.181Z"
updatedAt: "2022-10-31T16:50:26.520Z"
---