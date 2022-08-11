# hltv-stats

A database of hltv stats (matches, events, players, etc)

| 文件           | 数据      |
| ------------ | ------- |
| matches.json | []match |
| events.json  | []event |
| teams.json   | []team  |

# 数据结构 Data Structure

## 比赛 match

| 名称                  | 类型     | 含义              | 取值                                                                                            |
| ------------------- | ------ | --------------- | --------------------------------------------------------------------------------------------- |
| id                  | int    | 比赛ID            | 2297428                                                                                       |
| url                 | string | 比赛链接            | https://www.hltv.org/matches/2297428/dignitas-vs-dobrygaming-pgl-season-1-eu-qualifiers       |
| download_url        | string | 录像下载链接          | https://www.hltv.org/download/demo/18604                                                      |
| download_actual_url | string | 录像实际下载链接 | https://demos.hltv.org//demo/demofiles/demosection//PGLEUS1Q2-dignitas-vs-dobrygaming-bo5.rar |
| file_name           | string | 文件名             | PGLEUS1Q2-dignitas-vs-dobrygaming-bo5.rar                                                     |
| event_name          | string | 赛事名             | PGL Season 1 EU Qualifiers                                                                    |
| event_id            | int    | 赛事ID            | 1885                                                                                          |
| map_text            | string | 地图简写            | bo3                                                                                           |
| time                | string | unix时间          | 1439568000                                                                                    |
| team_a_score        | int    | 队伍A的分数          | 3                                                                                             |
| team_a_result       | string | 队伍A的结果          | won / lost / tie                                                                              |
| team_a_name         | string | 队伍A的名称          | Dignitas                                                                                      |
| team_a_id           | int    | 队伍A的ID          | 5422                                                       |
| team_b_score        | int    | 队伍B的分数          | 2                                                                                             |
| team_b_result       | string | 队伍B的结果          | lost / won / tie                                                                              |
| team_b_name         | string | 队伍B的名称          | Dobry Gaming                                                                                  |
| team_b_id           | int    | 队伍B的ID          | 5599                                                    |

## 赛事 event

| 名称         | 类型     | 含义        | 取值                                                                                                   |
| ---------- | ------ | --------- | ---------------------------------------------------------------------------------------------------- |
| id         | int    | 赛事ID      | 4616                                                                                                 |
| name       | string | 赛事名称      | Americas Minor North America Open Qualifier 2 - StarLadder Major 2019                                |
| url        | string | 赛事链接      | https://www.hltv.org/events/4616/americas-minor-north-america-open-qualifier-2-starladder-major-2019 |
| match_list | []int  | 赛事的所有比赛ID |                                                                                                      |

## 队伍 team

name和url可能并不准确

| 名称        | 类型     | 含义         |      |
| --------- | ------ | ---------- | ---- |
| id        | int    | 队伍ID       | 4869 |
| name      | string | 队伍名称       | ENCE |
| url       | string | 队伍链接       |      |
| flag_url  | string | 队伍国家/地区的链接 |      |
| flag_name | string | 队伍国家/地区名称  |      |
| logo      | string | 队伍LOGO     |      |
