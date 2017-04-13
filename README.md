# LearnUITableViewLayoutCell
使用UITableView+FDTemplateLayoutCell第三方自动适配返回cell高度
- 引用头文件
- #import "UITableView+FDTemplateLayoutCell.h"
# 手动布局使用自动适配'fd_enforceFrameLayout';
- cell.fd_enforceFrameLayout = YES; 需要设置为YES
# 返回高度
- [tableView fd_heightForCellWithIdentifier:<#(NSString *)#> configuration:<#^(id cell)configuration#>];
- [tableView fd_heightForCellWithIdentifier:<#(NSString *)#> cacheByIndexPath:<#(NSIndexPath *)#> configuration:<#^(id cell)configuration#>];
- [tableView fd_heightForCellWithIdentifier:<#(NSString *)#> cacheByKey:<#(id<NSCopying>)#> configuration:<#^(id cell)configuration#>];

# 在自动布局cell里面,可以不设置宽高,在设置布局的时候设置自己的宽/高/底等于自己宽/高/底make.width.equalTo(weakSelf.mas_width);

